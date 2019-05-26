# sub_401000 Function

The `sub_401000` function code of the Windows executable being reversed-engineered, as shown in IDA Pro:
    
    .text:00401000 ; ¦¦¦¦¦¦¦¦¦¦¦¦¦¦¦ S U B R O U T I N E ¦¦¦¦¦¦¦¦¦¦¦¦¦¦¦¦¦¦¦¦¦¦¦¦¦¦¦¦¦¦¦¦¦¦¦¦¦¦¦
    .text:00401000
    .text:00401000 ; Attributes: bp-based frame
    .text:00401000
    .text:00401000 proc            sub_401000 near         ; CODE XREF: _main+Dp
    .text:00401000                                         ; _main+1Fp ...
    .text:00401000
    .text:00401000 var_8           = dword ptr -8
    .text:00401000 var_4           = dword ptr -4
    .text:00401000 arg_0           = dword ptr  8 ; 0040A000 - offset of unk_40A000
    .text:00401000 arg_4           = dword ptr  0Ch ; 0040B9C0 - offset of szServerName
    .text:00401000
    .text:00401000                 push    ebp
    .text:00401001                 mov     ebp, esp
    .text:00401003                 sub     esp, 8 ; space being allocated for local variables
    .text:00401006                 mov     eax, [ebp+arg_0] ; eax = 0040A000h 
    .text:00401009                 movzx   ecx, [byte ptr eax] ; ecx = 8Ah 
    .text:0040100C                 movzx   edx, [byte_40A300] ; edx = 9h 
    .text:00401013                 xor     ecx, edx ; ecx = 83h
    .text:00401015                 and     ecx, 7Fh ; ecx = 3h
    .text:00401018                 mov     [ebp+var_8], ecx ; var_8 = ecx = 3h
    .text:0040101B                 mov     [ebp+var_4], 0 ; var_4 = 0h
    .text:00401022                 jmp     short loc_401036
    .text:00401024 ; ---------------------------------------------------------------------------
    .text:00401024
    .text:00401024 loc_401024:                             ; CODE XREF: sub_401000:loc_401072j
    .text:00401024                 mov     eax, [ebp+var_4] ; eax = var_4 = 0h -- 1h -- 2h
    .text:00401027                 add     eax, 1 ; eax = eax + 1 = 1h -- 2h -- 3h
    .text:0040102A                 mov     [ebp+var_4], eax ; var_4 = eax = 1h -- 2h -- 3h
    .text:0040102D                 mov     ecx, [ebp+var_8] ; ecx = var_8 = 3h -- 4h -- 5h
    .text:00401030                 add     ecx, 1 ; ecx = ecx + 1 = 4h -- 5h -- 6h
    .text:00401033                 mov     [ebp+var_8], ecx ; var_8 = ecx = 4h -- 5h -- 6h
    .text:00401036
    .text:00401036 loc_401036:                             ; CODE XREF: sub_401000+22j
    .text:00401036                 mov     edx, [ebp+arg_0] ; edx = 040A000h 
    .text:00401039                 add     edx, [ebp+var_8] ; edx = 040A000h + 3h = 040A003h -- 040A004h -- 040A005h
    .text:0040103C                 movzx   eax, [byte ptr edx] ; eax = CAh -- 7Dh -- E0h
    .text:0040103F                 mov     ecx, [ebp+var_8] ; ecx = var_8 = 3h -- 4h -- 5h
    .text:00401042                 and     ecx, 80000003h ; ecx = 3h AND 80000003h = 3h -- 0h -- 1h
    .text:00401048                 jns     short loc_40104F ; if s = 0 goto loc_40104F
    .text:0040104A                 dec     ecx ; ecx = ecx - 1
    .text:0040104B                 or      ecx, 0FFFFFFFCh ;
    .text:0040104E                 inc     ecx ; ecx = ecx + 1
    .text:0040104F
    .text:0040104F loc_40104F:                             ; CODE XREF: sub_401000+48j
    .text:0040104F                 movzx   edx, [byte_40A300+ecx] ; edx = 64h -- 9h -- 70h
    .text:00401056                 sub     eax, edx ; eax = eax - edx = CAh - 64h = 66h -- 74h -- 70h
    .text:00401058                 mov     ecx, [ebp+var_4] ; ecx = var_4 = 0h -- 1h -- 2h
    .text:0040105B                 mov     edx, [ebp+arg_4] ; edx = arg_4 = 0040B9C0
    .text:0040105E                 mov     [edx+ecx*2], ax ; mem[0040B9C0] = 66h (ascii: f) -- mem[0040B9C2] = 74h (ascii: t) -- mem[0040B9C4] = 70h (ascii: p), 2Eh(.), 75h(u), 63h(c), 64h(d), 2Eh(.), 69h(i), 65h(e)
    .text:00401062                 mov     eax, [ebp+var_4] ; eax = var_4 = 0h -- 1h -- 2h
    .text:00401065                 mov     ecx, [ebp+arg_4] ; ecx = 0040B9C0
    .text:00401068                 movzx   edx, [word ptr ecx+eax*2] ; 0066h -- 0074h -- 70h
    .text:0040106C                 test    edx, edx ; set Zf = 0
    .text:0040106E                 jnz     short loc_401072 ; if not zero (ie Zf = 0) go to 401072
    .text:00401070                 jmp     short loc_401074
    .text:00401072 ; ---------------------------------------------------------------------------
    .text:00401072
    .text:00401072 loc_401072:                             ; CODE XREF: sub_401000+6Ej
    .text:00401072                 jmp     short loc_401024 ; goto 401024
    .text:00401074 ; ---------------------------------------------------------------------------
    .text:00401074
    .text:00401074 loc_401074:                             ; CODE XREF: sub_401000+70j
    .text:00401074                 mov     esp, ebp
    .text:00401076                 pop     ebp
    .text:00401077                 retn
    .text:00401077 endp            sub_401000
    .text:00401077
    .text:00401077 ; ---------------------------------------------------------------------------