# Program Data Stored in Memory

Relevant snippets from the data region of the Windows executable being reversed-engineered, as shown in IDA Pro:

    
		.data:0040A000                 ;org 40A000h
    .data:0040A000 unk_40A000      db  8Ah ; è             ; DATA XREF: _main+8o
    .data:0040A001                 db  48h ; H
    .data:0040A002                 db 0FEh ; ¦
    .data:0040A003                 db 0CAh ; -
    .data:0040A004                 db  7Dh ; }
    .data:0040A005                 db 0E0h ; a
    .data:0040A006                 db  99h ; Ö
    .data:0040A007                 db 0D9h ; +
    .data:0040A008                 db  6Ch ; l
    .data:0040A009                 db 0D4h ; +
    .data:0040A00A                 db  99h ; Ö
    .data:0040A00B                 db 0CDh ; -
    .data:0040A00C                 db  6Eh ; n
    .data:0040A00D                 db  70h ; p
    .data:0040A00E                 db  7Bh ; {
    .data:0040A00F                 db 0B1h ; ¦
    .data:0040A010                 db  6Fh ; o
    .data:0040A011                 db  84h ; ä
    .data:0040A012                 db 0D3h ; +
    .data:0040A013                 db  9Fh ; ƒ
    .data:0040A014                 db  25h ; %
    .data:0040A015                 db  48h ; H
    .data:0040A016                 db 0AFh ; »
    .data:0040A017                 db    5
    .data:0040A018                 db 0AEh ; «
    .data:0040A019                 db  9Ah ; Ü
    .data:0040A01A                 db 0AAh ; ¬
    .data:0040A01B                 db  82h ; é
    .data:0040A01C                 db  8Eh ; Ä
    .data:0040A01D                 db 0F5h ; )
    .data:0040A01E                 db  89h ; ë
    .data:0040A01F                 db  77h ; w
    .data:0040A020                 db 0ECh ; 8
    .data:0040A021                 db  6Bh ; k
    .data:0040A022                 db 0C1h ; -
    .data:0040A023                 db  31h ; 1
    .data:0040A024                 db 0FAh ; ·
    .data:0040A025                 db 0B8h ; +
    .data:0040A026                 db 0D6h ; +
    .data:0040A027                 db  3Ch ; <
    .data:0040A028                 db  35h ; 5
    .data:0040A029                 db 0E4h ; S
    .data:0040A02A                 db  10h
    .data:0040A02B                 db  72h ; r
    .data:0040A02C                 db 0A1h ; í
    .data:0040A02D                 db 0C4h ; -
    .data:0040A02E                 db  71h ; q
    .data:0040A02F                 db 0F7h ; ˜
    .data:0040A030                 db  0Fh
    .data:0040A031                 db  18h
    .data:0040A032                 db  7Eh ; ~
    .data:0040A033                 db 0BCh ; +
    .data:0040A034                 db 0FBh ; v
    .data:0040A035                 db  99h ; Ö
    .data:0040A036                 db  17h
    .data:0040A037                 db 0B1h ; ¦
    .data:0040A038                 db 0A9h ; ¬
    .data:0040A039                 db  26h ; &
    .data:0040A03A                 db  90h ; É
    .data:0040A03B                 db  50h ; P
    .data:0040A03C                 db 0F8h ; °
    .data:0040A03D                 db 0E3h ; p
    .data:0040A03E                 db 0D1h ; -
    .data:0040A03F                 db  93h ; ô
    .data:0040A040                 db  9Dh ; ¥
    .data:0040A041                 db    9
    .data:0040A042                 db  11h
    .data:0040A043                 db  1Ah
    .data:0040A044                 db 0C4h ; -
    .data:0040A045                 db  28h ; (
    .data:0040A046                 db 0F9h ; ·
    .data:0040A047                 db  78h ; x
    .data:0040A048                 db  3Ah ; :
    .data:0040A049                 db  25h ; %
    .data:0040A04A                 db 0DCh ; _
    .data:0040A04B                 db 0F6h ; ÷
    .data:0040A04C                 db  22h ; "
    .data:0040A04D                 db  3Ch ; <
    .data:0040A04E                 db  38h ; 8
    .data:0040A04F                 db 0D1h ; -
    .data:0040A050                 db  64h ; d
    .data:0040A051                 db 0AFh ; »
    .data:0040A052                 db  2Bh ; +
    .data:0040A053                 db  2Fh ; /
    .data:0040A054                 db 0CBh ; -
    .data:0040A055                 db  18h
    .data:0040A056                 db 0A6h ; ª
    .data:0040A057                 db  53h ; S
    .data:0040A058                 db    3
    .data:0040A059                 db  62h ; b
    .data:0040A05A                 db  76h ; v
    .data:0040A05B                 db  59h ; Y
    .data:0040A05C                 db 0EEh ; e
    .data:0040A05D                 db  71h ; q
    .data:0040A05E                 db  75h ; u
    .data:0040A05F                 db 0F4h ; (
    .data:0040A060                 db  82h ; é
    .data:0040A061                 db  81h ; ü
    .data:0040A062                 db  70h ; p
    .data:0040A063                 db 0FCh ; n
    .data:0040A064                 db  2Eh ; .
    .data:0040A065                 db 0A7h ; º
    .data:0040A066                 db 0ABh ; ½
    .data:0040A067                 db  44h ; D
    .data:0040A068                 db 0DCh ; _
    .data:0040A069                 db  2Bh ; +
    .data:0040A06A                 db 0FDh ; ²
    .data:0040A06B                 db  0Dh
    .data:0040A06C                 db 0BBh ; +
    .data:0040A06D                 db 0FCh ; n
    .data:0040A06E                 db 0EBh ; d
    .data:0040A06F                 db  86h ; å
    .data:0040A070                 db  3Ch ; <
    .data:0040A071                 db  84h ; ä
    .data:0040A072                 db 0CEh ; +
    .data:0040A073                 db  32h ; 2
    .data:0040A074                 db  7Fh ; 
    .data:0040A075                 db  28h ; (
    .data:0040A076                 db 0D3h ; +
    .data:0040A077                 db 0A3h ; ú
    .data:0040A078                 db  2Ah ; *
    .data:0040A079                 db  26h ; &
    .data:0040A07A                 db  7Eh ; ~
    .data:0040A07B                 db 0DFh ; ¯
    .data:0040A07C                 db 0C9h ; +
    .data:0040A07D                 db 0AFh ; »
    .data:0040A07E                 db  62h ; b
    .data:0040A07F                 db  6Bh ; k
    .data:0040A080                 db 0CAh ; -
    .data:0040A081                 db  64h ; d
    .data:0040A082                 db 0C7h ; ¦
    .data:0040A083                 db  3Dh ; =
    .data:0040A084                 db  1Fh
    .data:0040A085                 db  94h ; ö
    .data:0040A086                 db  75h ; u
    .data:0040A087                 db  25h ; %
    .data:0040A088                 db 0ACh ; ¼
    .data:0040A089                 db  65h ; e
    .data:0040A08A                 db 0C4h ; -
    .data:0040A08B                 db 0E1h ; ß
    .data:0040A08C                 db  8Ah ; è
    .data:0040A08D                 db  50h ; P
    .data:0040A08E                 db  50h ; P
    .data:0040A08F                 db 0F0h ; =
    .data:0040A090                 db 0A8h ; ¿
    .data:0040A091                 db    2
    .data:0040A092                 db  44h ; D
    .data:0040A093                 db  58h ; X
    .data:0040A094                 db    4
    .data:0040A095                 db  9Fh ; ƒ
    .data:0040A096                 db  3Ch ; <
    .data:0040A097                 db 0F2h ; =
    .data:0040A098                 db 0D0h ; -
    .data:0040A099                 db  79h ; y
    .data:0040A09A                 db 0AAh ; ¬
    .data:0040A09B                 db  7Ah ; z
    .data:0040A09C                 db  6Bh ; k
    .data:0040A09D                 db  21h ; !
    .data:0040A09E                 db 0AEh ; «
    .data:0040A09F                 db  5Ch ; \
    .data:0040A0A0                 db 0E8h ; F
    .data:0040A0A1                 db  7Ch ; |
    .data:0040A0A2                 db 0E3h ; p
    .data:0040A0A3                 db  98h ; ÿ
    .data:0040A0A4                 db  0Bh
    .data:0040A0A5                 db  41h ; A
    .data:0040A0A6                 db    3
    .data:0040A0A7                 db 0B3h ; ¦
    .data:0040A0A8                 db 0FEh ; ¦
    .data:0040A0A9                 db 0F8h ; °
    .data:0040A0AA                 db 0E7h ; t
    .data:0040A0AB                 db  74h ; t
    .data:0040A0AC                 db 0AEh ; «
    .data:0040A0AD                 db  74h ; t
    .data:0040A0AE                 db  4Ah ; J
    .data:0040A0AF                 db 0FCh ; n
    .data:0040A0B0                 db  7Fh ; 
    .data:0040A0B1                 db 0C8h ; +
    .data:0040A0B2                 db  4Bh ; K
    .data:0040A0B3                 db  84h ; ä
    .data:0040A0B4                 db  4Ah ; J
    .data:0040A0B5                 db  49h ; I
    .data:0040A0B6                 db  1Dh
    .data:0040A0B7                 db  23h ; #
    .data:0040A0B8                 db  6Ch ; l
    .data:0040A0B9                 db  9Ah ; Ü
    .data:0040A0BA                 db 0E1h ; ß
    .data:0040A0BB                 db  91h ; æ
    .data:0040A0BC                 db  33h ; 3
    .data:0040A0BD                 db 0BDh ; +
    .data:0040A0BE                 db  10h
    .data:0040A0BF                 db 0BDh ; +
    .data:0040A0C0                 db  15h
    .data:0040A0C1                 db  40h ; @
    .data:0040A0C2                 db 0F4h ; (
    .data:0040A0C3                 db  1Dh
    .data:0040A0C4                 db 0E2h ; G
    .data:0040A0C5                 db  70h ; p
    .data:0040A0C6                 db  27h ; '
    .data:0040A0C7                 db  9Dh ; ¥
    .data:0040A0C8                 db  6Ah ; j
    .data:0040A0C9                 db  3Dh ; =
    .data:0040A0CA                 db 0FEh ; ¦
    .data:0040A0CB                 db  98h ; ÿ
    .data:0040A0CC                 db  4Ch ; L
    .data:0040A0CD                 db  9Ch ; £
    .data:0040A0CE                 db  62h ; b
    .data:0040A0CF                 db  30h ; 0
    .data:0040A0D0                 db  58h ; X
    .data:0040A0D1                 db  2Eh ; .
    .data:0040A0D2                 db    4
    .data:0040A0D3                 db 0F0h ; =
    .data:0040A0D4                 db 0C9h ; +
    .data:0040A0D5                 db 0E5h ; s
    .data:0040A0D6                 db 0D9h ; +
    .data:0040A0D7                 db  2Eh ; .
    .data:0040A0D8                 db  37h ; 7
    .data:0040A0D9                 db 0FBh ; v
    .data:0040A0DA                 db 0F0h ; =
    .data:0040A0DB                 db  64h ; d
    .data:0040A0DC                 db  0Ah
    .data:0040A0DD                 db 0F2h ; =
    .data:0040A0DE                 db 0E3h ; p
    .data:0040A0DF                 db  1Eh
    .data:0040A0E0                 db 0CAh ; -
    .data:0040A0E1                 db  60h ; `
    .data:0040A0E2                 db  10h
    .data:0040A0E3                 db  2Ch ; ,
    .data:0040A0E4                 db  9Eh ; P
    .data:0040A0E5                 db  5Eh ; ^
    .data:0040A0E6                 db 0D5h ; +
    .data:0040A0E7                 db  24h ; $
    .data:0040A0E8                 db 0CCh ; ¦
    .data:0040A0E9                 db  3Ch ; <
    .data:0040A0EA                 db    9
    .data:0040A0EB                 db 0F5h ; )
    .data:0040A0EC                 db  8Dh ; ì
    .data:0040A0ED                 db 0EEh ; e
    .data:0040A0EE                 db  49h ; I
    .data:0040A0EF                 db  1Eh
    .data:0040A0F0                 db  11h
    .data:0040A0F1                 db  3Ah ; :
    .data:0040A0F2                 db  76h ; v
    .data:0040A0F3                 db 0A9h ; ¬
    .data:0040A0F4                 db 0F9h ; ·
    .data:0040A0F5                 db  26h ; &
    .data:0040A0F6                 db 0F8h ; °
    .data:0040A0F7                 db  9Dh ; ¥
    .data:0040A0F8                 db  31h ; 1
    .data:0040A0F9                 db  41h ; A
    .data:0040A0FA                 db    6
    .data:0040A0FB                 db  83h ; â
    .data:0040A0FC                 db  59h ; Y
    .data:0040A0FD                 db  1Fh
    .data:0040A0FE                 db  2Ah ; *
    .data:0040A0FF                 db    0
    
    .data:0040A300 byte_40A300     db 9                    ; DATA XREF: sub_401000+Cr
    .data:0040A300                                         ; sub_401000:loc_40104Fr
    .data:0040A301                 db  70h ; p
    .data:0040A302                 db  6Bh ; k
    .data:0040A303                 db  64h ; d
    .data:0040A304                 db    0
    .data:0040A305                 db    0
    .data:0040A306                 db    0
    .data:0040A307                 db    0
    
    .data:0040B9C0 ; const WCHAR szServerName
    .data:0040B9C0 szServerName    dw 99                    ; DATA XREF: sub_401080+3Eo
    .data:0040B9C0                                         ; sub_401160+3Eo ...
    .data:0040B9C2                 db    9
    .data:0040B9C3                 db    F
    .data:0040B9C4                 db    0
    .data:0040B9C5                 db    0
    .data:0040B9C6                 db    0
    .data:0040B9C7                 db    0
    .data:0040B9C8                 db    0
    .data:0040B9C9                 db    0
    .data:0040B9CA                 db    0
    .data:0040B9CB                 db    0
    .data:0040B9CC                 db    0
    .data:0040B9CD                 db    0
    .data:0040B9CE                 db    0
    .data:0040B9CF                 db    0
    .data:0040B9D0                 db    0
    .data:0040B9D1                 db    0
    .data:0040B9D2                 db    0
    .data:0040B9D3                 db    0
    .data:0040B9D4                 db    0
    .data:0040B9D5                 db    0
    .data:0040B9D6                 db    0
    .data:0040B9D7                 db    0
    .data:0040B9D8                 db    0
    .data:0040B9D9                 db    0
    .data:0040B9DA                 db    0
    .data:0040B9DB                 db    0
    .data:0040B9DC                 db    0
    .data:0040B9DD                 db    0
    .data:0040B9DE                 db    0
    .data:0040B9DF                 db    0
    .data:0040B9E0                 db    0
    .data:0040B9E1                 db    0
    .data:0040B9E2                 db    0
    .data:0040B9E3                 db    0
    .data:0040B9E4                 db    0
    .data:0040B9E5                 db    0
    .data:0040B9E6                 db    0
    .data:0040B9E7                 db    0
    .data:0040B9E8                 db    0
    .data:0040B9E9                 db    0
    .data:0040B9EA                 db    0
    .data:0040B9EB                 db    0
    .data:0040B9EC                 db    0
    .data:0040B9ED                 db    0
    .data:0040B9EE                 db    0
    .data:0040B9EF                 db    0
    .data:0040B9F0                 db    0
    .data:0040B9F1                 db    0
    .data:0040B9F2                 db    0
    .data:0040B9F3                 db    0
    .data:0040B9F4                 db    0
    .data:0040B9F5                 db    0
    .data:0040B9F6                 db    0
    .data:0040B9F7                 db    0
    .data:0040B9F8                 db    0
    .data:0040B9F9                 db    0
    .data:0040B9FA                 db    0
    .data:0040B9FB                 db    0
    .data:0040B9FC                 db    0
    .data:0040B9FD                 db    0
    .data:0040B9FE                 db    0
    .data:0040B9FF                 db    0
    .data:0040BA00                 db    0
    .data:0040BA01                 db    0
    .data:0040BA02                 db    0
    .data:0040BA03                 db    0
    .data:0040BA04                 db    0
    .data:0040BA05                 db    0
    .data:0040BA06                 db    0
    .data:0040BA07                 db    0
    .data:0040BA08                 db    0
    .data:0040BA09                 db    0
    .data:0040BA0A                 db    0
    .data:0040BA0B                 db    0
    .data:0040BA0C                 db    0
    .data:0040BA0D                 db    0
    .data:0040BA0E                 db    0
    .data:0040BA0F                 db    0
    .data:0040BA10                 db    0
    .data:0040BA11                 db    0
    .data:0040BA12                 db    0
    .data:0040BA13                 db    0
    .data:0040BA14                 db    0
    .data:0040BA15                 db    0
    .data:0040BA16                 db    0
    .data:0040BA17                 db    0
    .data:0040BA18                 db    0
    .data:0040BA19                 db    0
    .data:0040BA1A                 db    0
    .data:0040BA1B                 db    0
    .data:0040BA1C                 db    0
    .data:0040BA1D                 db    0
    .data:0040BA1E                 db    0
    .data:0040BA1F                 db    0
    .data:0040BA20                 db    0
    .data:0040BA21                 db    0
    .data:0040BA22                 db    0
    .data:0040BA23                 db    0
    .data:0040BA24                 db    0
    .data:0040BA25                 db    0
    .data:0040BA26                 db    0
    .data:0040BA27                 db    0
    .data:0040BA28                 db    0
    .data:0040BA29                 db    0
    .data:0040BA2A                 db    0
    .data:0040BA2B                 db    0
    .data:0040BA2C                 db    0
    .data:0040BA2D                 db    0
    .data:0040BA2E                 db    0
    .data:0040BA2F                 db    0
    .data:0040BA30                 db    0
    .data:0040BA31                 db    0
    .data:0040BA32                 db    0
    .data:0040BA33                 db    0
    .data:0040BA34                 db    0
    .data:0040BA35                 db    0
    .data:0040BA36                 db    0
    .data:0040BA37                 db    0
    .data:0040BA38                 db    0
    .data:0040BA39                 db    0
    .data:0040BA3A                 db    0
    .data:0040BA3B                 db    0
    .data:0040BA3C                 db    0
    .data:0040BA3D                 db    0
    .data:0040BA3E                 db    0
    .data:0040BA3F                 db    0
    .data:0040BA40                 db    0
    .data:0040BA41                 db    0
    .data:0040BA42                 db    0
    .data:0040BA43                 db    0
    .data:0040BA44                 db    0
    .data:0040BA45                 db    0
    .data:0040BA46                 db    0
    .data:0040BA47                 db    0
    .data:0040BA48                 db    0
    .data:0040BA49                 db    0
    .data:0040BA4A                 db    0
    .data:0040BA4B                 db    0
    .data:0040BA4C                 db    0
    .data:0040BA4D                 db    0
    .data:0040BA4E                 db    0
    .data:0040BA4F                 db    0
    .data:0040BA50                 db    0
    .data:0040BA51                 db    0
    .data:0040BA52                 db    0
    .data:0040BA53                 db    0
    .data:0040BA54                 db    0
    .data:0040BA55                 db    0
    .data:0040BA56                 db    0
    .data:0040BA57                 db    0
    .data:0040BA58                 db    0
    .data:0040BA59                 db    0
    .data:0040BA5A                 db    0
    .data:0040BA5B                 db    0
    .data:0040BA5C                 db    0
    .data:0040BA5D                 db    0
    .data:0040BA5E                 db    0
    .data:0040BA5F                 db    0
    .data:0040BA60                 db    0
    .data:0040BA61                 db    0
    .data:0040BA62                 db    0
    .data:0040BA63                 db    0
    .data:0040BA64                 db    0
    .data:0040BA65                 db    0
    .data:0040BA66                 db    0
    .data:0040BA67                 db    0
    .data:0040BA68                 db    0
    .data:0040BA69                 db    0
    .data:0040BA6A                 db    0
    .data:0040BA6B                 db    0
    .data:0040BA6C                 db    0
    .data:0040BA6D                 db    0
    .data:0040BA6E                 db    0
    .data:0040BA6F                 db    0
    .data:0040BA70                 db    0
    .data:0040BA71                 db    0
    .data:0040BA72                 db    0
    .data:0040BA73                 db    0
    .data:0040BA74                 db    0
    .data:0040BA75                 db    0
    .data:0040BA76                 db    0
    .data:0040BA77                 db    0
    .data:0040BA78                 db    0
    .data:0040BA79                 db    0
    .data:0040BA7A                 db    0
    .data:0040BA7B                 db    0
    .data:0040BA7C                 db    0
    .data:0040BA7D                 db    0
    .data:0040BA7E                 db    0
    .data:0040BA7F                 db    0
    .data:0040BA80                 db    0
    .data:0040BA81                 db    0
    .data:0040BA82                 db    0
    .data:0040BA83                 db    0
    .data:0040BA84                 db    0
    .data:0040BA85                 db    0
    .data:0040BA86                 db    0
    .data:0040BA87                 db    0
    .data:0040BA88                 db    0
    .data:0040BA89                 db    0
    .data:0040BA8A                 db    0
    .data:0040BA8B                 db    0
    .data:0040BA8C                 db    0
    .data:0040BA8D                 db    0
    .data:0040BA8E                 db    0
    .data:0040BA8F                 db    0
    .data:0040BA90                 db    0
    .data:0040BA91                 db    0
    .data:0040BA92                 db    0
    .data:0040BA93                 db    0
    .data:0040BA94                 db    0
    .data:0040BA95                 db    0
    .data:0040BA96                 db    0
    .data:0040BA97                 db    0
    .data:0040BA98                 db    0
    .data:0040BA99                 db    0
    .data:0040BA9A                 db    0
    .data:0040BA9B                 db    0
    .data:0040BA9C                 db    0
    .data:0040BA9D                 db    0
    .data:0040BA9E                 db    0
    .data:0040BA9F                 db    0
    .data:0040BAA0                 db    0
    .data:0040BAA1                 db    0
    .data:0040BAA2                 db    0
    .data:0040BAA3                 db    0
    .data:0040BAA4                 db    0
    .data:0040BAA5                 db    0
    .data:0040BAA6                 db    0
    .data:0040BAA7                 db    0
    .data:0040BAA8                 db    0
    .data:0040BAA9                 db    0
    .data:0040BAAA                 db    0
    .data:0040BAAB                 db    0
    .data:0040BAAC                 db    0
    .data:0040BAAD                 db    0
    .data:0040BAAE                 db    0
    .data:0040BAAF                 db    0
    .data:0040BAB0                 db    0
    .data:0040BAB1                 db    0
    .data:0040BAB2                 db    0
    .data:0040BAB3                 db    0
    .data:0040BAB4                 db    0
    .data:0040BAB5                 db    0
    .data:0040BAB6                 db    0
    .data:0040BAB7                 db    0
    .data:0040BAB8                 db    0
    .data:0040BAB9                 db    0
    .data:0040BABA                 db    0
    .data:0040BABB                 db    0
    .data:0040BABC                 db    0
    .data:0040BABD                 db    0
    .data:0040BABE                 db    0
    .data:0040BABF                 db    0
    .data:0040BAC0                 db    0
    .data:0040BAC1                 db    0
    .data:0040BAC2                 db    0
    .data:0040BAC3                 db    0
    .data:0040BAC4                 db    0
    .data:0040BAC5                 db    0
    .data:0040BAC6                 db    0
    .data:0040BAC7                 db    0
    .data:0040BAC8                 db    0
    .data:0040BAC9                 db    0
    .data:0040BACA                 db    0
    .data:0040BACB                 db    0
    .data:0040BACC                 db    0
    .data:0040BACD                 db    0
    .data:0040BACE                 db    0
    .data:0040BACF                 db    0
    .data:0040BAD0                 db    0
    .data:0040BAD1                 db    0
    .data:0040BAD2                 db    0
    .data:0040BAD3                 db    0
    .data:0040BAD4                 db    0
    .data:0040BAD5                 db    0
    .data:0040BAD6                 db    0
    .data:0040BAD7                 db    0
    .data:0040BAD8                 db    0
    .data:0040BAD9                 db    0
    .data:0040BADA                 db    0
    .data:0040BADB                 db    0
    .data:0040BADC                 db    0
    .data:0040BADD                 db    0
    .data:0040BADE                 db    0
    .data:0040BADF                 db    0
    .data:0040BAE0                 db    0
    .data:0040BAE1                 db    0
    .data:0040BAE2                 db    0
    .data:0040BAE3                 db    0
    .data:0040BAE4                 db    0
    .data:0040BAE5                 db    0
    .data:0040BAE6                 db    0
    .data:0040BAE7                 db    0
    .data:0040BAE8                 db    0
    .data:0040BAE9                 db    0
    .data:0040BAEA                 db    0
    .data:0040BAEB                 db    0
    .data:0040BAEC                 db    0
    .data:0040BAED                 db    0
    .data:0040BAEE                 db    0
    .data:0040BAEF                 db    0
    .data:0040BAF0                 db    0
    .data:0040BAF1                 db    0
    .data:0040BAF2                 db    0
    .data:0040BAF3                 db    0
    .data:0040BAF4                 db    0
    .data:0040BAF5                 db    0
    .data:0040BAF6                 db    0
    .data:0040BAF7                 db    0
    .data:0040BAF8                 db    0
    .data:0040BAF9                 db    0
    .data:0040BAFA                 db    0
    .data:0040BAFB                 db    0
    .data:0040BAFC                 db    0
    .data:0040BAFD                 db    0
    .data:0040BAFE                 db    0
    .data:0040BAFF                 db    0
    .data:0040BB00                 db    0
    .data:0040BB01                 db    0
    .data:0040BB02                 db    0
    .data:0040BB03                 db    0
    .data:0040BB04                 db    0
    .data:0040BB05                 db    0
    .data:0040BB06                 db    0
    .data:0040BB07                 db    0
    .data:0040BB08                 db    0
    .data:0040BB09                 db    0
    .data:0040BB0A                 db    0
    .data:0040BB0B                 db    0
    .data:0040BB0C                 db    0
    .data:0040BB0D                 db    0
    .data:0040BB0E                 db    0
    .data:0040BB0F                 db    0
    .data:0040BB10                 db    0
    .data:0040BB11                 db    0
    .data:0040BB12                 db    0
    .data:0040BB13                 db    0
    .data:0040BB14                 db    0
    .data:0040BB15                 db    0
    .data:0040BB16                 db    0
    .data:0040BB17                 db    0
    .data:0040BB18                 db    0
    .data:0040BB19                 db    0
    .data:0040BB1A                 db    0
    .data:0040BB1B                 db    0
    .data:0040BB1C                 db    0
    .data:0040BB1D                 db    0
    .data:0040BB1E                 db    0
    .data:0040BB1F                 db    0
    .data:0040BB20                 db    0
    .data:0040BB21                 db    0
    .data:0040BB22                 db    0
    .data:0040BB23                 db    0
    .data:0040BB24                 db    0
    .data:0040BB25                 db    0
    .data:0040BB26                 db    0
    .data:0040BB27                 db    0
    .data:0040BB28                 db    0
    .data:0040BB29                 db    0
    .data:0040BB2A                 db    0
    .data:0040BB2B                 db    0
    .data:0040BB2C                 db    0
    .data:0040BB2D                 db    0
    .data:0040BB2E                 db    0
    .data:0040BB2F                 db    0
    .data:0040BB30                 db    0
    .data:0040BB31                 db    0
    .data:0040BB32                 db    0
    .data:0040BB33                 db    0
    .data:0040BB34                 db    0
    .data:0040BB35                 db    0
    .data:0040BB36                 db    0
    .data:0040BB37                 db    0
    .data:0040BB38                 db    0
    .data:0040BB39                 db    0
    .data:0040BB3A                 db    0
    .data:0040BB3B                 db    0
    .data:0040BB3C                 db    0
    .data:0040BB3D                 db    0
    .data:0040BB3E                 db    0
    .data:0040BB3F                 db    0
    .data:0040BB40                 db    0
    .data:0040BB41                 db    0
    .data:0040BB42                 db    0
    .data:0040BB43                 db    0
    .data:0040BB44                 db    0
    .data:0040BB45                 db    0
    .data:0040BB46                 db    0
    .data:0040BB47                 db    0
    .data:0040BB48                 db    0
    .data:0040BB49                 db    0
    .data:0040BB4A                 db    0
    .data:0040BB4B                 db    0
    .data:0040BB4C                 db    0
    .data:0040BB4D                 db    0
    .data:0040BB4E                 db    0
    .data:0040BB4F                 db    0
    .data:0040BB50                 db    0
    .data:0040BB51                 db    0
    .data:0040BB52                 db    0
    .data:0040BB53                 db    0
    .data:0040BB54                 db    0
    .data:0040BB55                 db    0
    .data:0040BB56                 db    0
    .data:0040BB57                 db    0
    .data:0040BB58                 db    0
    .data:0040BB59                 db    0
    .data:0040BB5A                 db    0
    .data:0040BB5B                 db    0
    .data:0040BB5C                 db    0
    .data:0040BB5D                 db    0
    .data:0040BB5E                 db    0
    .data:0040BB5F                 db    0
    .data:0040BB60                 db    0
    .data:0040BB61                 db    0
    .data:0040BB62                 db    0
    .data:0040BB63                 db    0
    .data:0040BB64                 db    0
    .data:0040BB65                 db    0
    .data:0040BB66                 db    0
    .data:0040BB67                 db    0
    .data:0040BB68                 db    0
    .data:0040BB69                 db    0
    .data:0040BB6A                 db    0
    .data:0040BB6B                 db    0
    .data:0040BB6C                 db    0
    .data:0040BB6D                 db    0
    .data:0040BB6E                 db    0
    .data:0040BB6F                 db    0
    .data:0040BB70                 db    0
    .data:0040BB71                 db    0
    .data:0040BB72                 db    0
    .data:0040BB73                 db    0
    .data:0040BB74                 db    0
    .data:0040BB75                 db    0
    .data:0040BB76                 db    0
    .data:0040BB77                 db    0
    .data:0040BB78                 db    0
    .data:0040BB79                 db    0
    .data:0040BB7A                 db    0
    .data:0040BB7B                 db    0
    .data:0040BB7C                 db    0
    .data:0040BB7D                 db    0
    .data:0040BB7E                 db    0
    .data:0040BB7F                 db    0
    .data:0040BB80                 db    0
    .data:0040BB81                 db    0
    .data:0040BB82                 db    0
    .data:0040BB83                 db    0
    .data:0040BB84                 db    0
    .data:0040BB85                 db    0
    .data:0040BB86                 db    0
    .data:0040BB87                 db    0
    .data:0040BB88                 db    0
    .data:0040BB89                 db    0
    .data:0040BB8A                 db    0
    .data:0040BB8B                 db    0
    .data:0040BB8C                 db    0
    .data:0040BB8D                 db    0
    .data:0040BB8E                 db    0
    .data:0040BB8F                 db    0
    .data:0040BB90                 db    0
    .data:0040BB91                 db    0
    .data:0040BB92                 db    0
    .data:0040BB93                 db    0
    .data:0040BB94                 db    0
    .data:0040BB95                 db    0
    .data:0040BB96                 db    0
    .data:0040BB97                 db    0
    .data:0040BB98                 db    0
    .data:0040BB99                 db    0
    .data:0040BB9A                 db    0
    .data:0040BB9B                 db    0
    .data:0040BB9C                 db    0
    .data:0040BB9D                 db    0
    .data:0040BB9E                 db    0
    .data:0040BB9F                 db    0
    .data:0040BBA0                 db    0
    .data:0040BBA1                 db    0
    .data:0040BBA2                 db    0
    .data:0040BBA3                 db    0
    .data:0040BBA4                 db    0
    .data:0040BBA5                 db    0
    .data:0040BBA6                 db    0
    .data:0040BBA7                 db    0
    .data:0040BBA8                 db    0
    .data:0040BBA9                 db    0
    .data:0040BBAA                 db    0
    .data:0040BBAB                 db    0
    .data:0040BBAC                 db    0
    .data:0040BBAD                 db    0
    .data:0040BBAE                 db    0
    .data:0040BBAF                 db    0
    .data:0040BBB0                 db    0
    .data:0040BBB1                 db    0
    .data:0040BBB2                 db    0
    .data:0040BBB3                 db    0
    .data:0040BBB4                 db    0
    .data:0040BBB5                 db    0
    .data:0040BBB6                 db    0
    .data:0040BBB7                 db    0
    .data:0040BBB8                 db    0
    .data:0040BBB9                 db    0
    .data:0040BBBA                 db    0
    .data:0040BBBB                 db    0
    .data:0040BBBC                 db    0
    .data:0040BBBD                 db    0
    .data:0040BBBE                 db    0
    .data:0040BBBF                 db    0
    
    .data:0040B3C0 ; const WCHAR szUserName
    .data:0040B3C0 szUserName      dw 0                    ; DATA XREF: sub_401080+37o
    .data:0040B3C0                                         ; sub_401160+37o ...
    .data:0040B3C2                 db    0
    .data:0040B3C3                 db    0
    .data:0040B3C4                 db    0
    .data:0040B3C5                 db    0
    .data:0040B3C6                 db    0
    .data:0040B3C7                 db    0
    .data:0040B3C8                 db    0
    .data:0040B3C9                 db    0
    .data:0040B3CA                 db    0
    .data:0040B3CB                 db    0
    .data:0040B3CC                 db    0
    .data:0040B3CD                 db    0
    .data:0040B3CE                 db    0
    .data:0040B3CF                 db    0
    .data:0040B3D0                 db    0
    .data:0040B3D1                 db    0
    .data:0040B3D2                 db    0
    .data:0040B3D3                 db    0
    .data:0040B3D4                 db    0
    .data:0040B3D5                 db    0
    .data:0040B3D6                 db    0
    .data:0040B3D7                 db    0
    .data:0040B3D8                 db    0
    .data:0040B3D9                 db    0
    .data:0040B3DA                 db    0
    .data:0040B3DB                 db    0
    .data:0040B3DC                 db    0
    .data:0040B3DD                 db    0
    .data:0040B3DE                 db    0
    .data:0040B3DF                 db    0
    .data:0040B3E0                 db    0
    .data:0040B3E1                 db    0
    .data:0040B3E2                 db    0
    .data:0040B3E3                 db    0
    .data:0040B3E4                 db    0
    .data:0040B3E5                 db    0
    .data:0040B3E6                 db    0
    .data:0040B3E7                 db    0
    .data:0040B3E8                 db    0
    .data:0040B3E9                 db    0
    .data:0040B3EA                 db    0
    .data:0040B3EB                 db    0
    .data:0040B3EC                 db    0
    .data:0040B3ED                 db    0
    .data:0040B3EE                 db    0
    .data:0040B3EF                 db    0
    .data:0040B3F0                 db    0
    .data:0040B3F1                 db    0
    .data:0040B3F2                 db    0
    .data:0040B3F3                 db    0
    .data:0040B3F4                 db    0
    .data:0040B3F5                 db    0
    .data:0040B3F6                 db    0
    .data:0040B3F7                 db    0
    .data:0040B3F8                 db    0
    .data:0040B3F9                 db    0
    .data:0040B3FA                 db    0
    .data:0040B3FB                 db    0
    .data:0040B3FC                 db    0
    .data:0040B3FD                 db    0
    .data:0040B3FE                 db    0
    .data:0040B3FF                 db    0
    .data:0040B400                 db    0
    .data:0040B401                 db    0
    .data:0040B402                 db    0
    .data:0040B403                 db    0
    .data:0040B404                 db    0
    .data:0040B405                 db    0
    .data:0040B406                 db    0
    .data:0040B407                 db    0
    .data:0040B408                 db    0
    .data:0040B409                 db    0
    .data:0040B40A                 db    0
    .data:0040B40B                 db    0
    .data:0040B40C                 db    0
    .data:0040B40D                 db    0
    .data:0040B40E                 db    0
    .data:0040B40F                 db    0
    .data:0040B410                 db    0
    .data:0040B411                 db    0
    .data:0040B412                 db    0
    .data:0040B413                 db    0
    .data:0040B414                 db    0
    .data:0040B415                 db    0
    .data:0040B416                 db    0
    .data:0040B417                 db    0
    .data:0040B418                 db    0
    .data:0040B419                 db    0
    .data:0040B41A                 db    0
    .data:0040B41B                 db    0
    .data:0040B41C                 db    0
    .data:0040B41D                 db    0
    .data:0040B41E                 db    0
    .data:0040B41F                 db    0
    .data:0040B420                 db    0
    .data:0040B421                 db    0
    .data:0040B422                 db    0
    .data:0040B423                 db    0
    .data:0040B424                 db    0
    .data:0040B425                 db    0
    .data:0040B426                 db    0
    .data:0040B427                 db    0
    .data:0040B428                 db    0
    .data:0040B429                 db    0
    .data:0040B42A                 db    0
    .data:0040B42B                 db    0
    .data:0040B42C                 db    0
    .data:0040B42D                 db    0
    .data:0040B42E                 db    0
    .data:0040B42F                 db    0
    .data:0040B430                 db    0
    .data:0040B431                 db    0
    .data:0040B432                 db    0
    .data:0040B433                 db    0
    .data:0040B434                 db    0
    .data:0040B435                 db    0
    .data:0040B436                 db    0
    .data:0040B437                 db    0
    .data:0040B438                 db    0
    .data:0040B439                 db    0
    .data:0040B43A                 db    0
    .data:0040B43B                 db    0
    .data:0040B43C                 db    0
    .data:0040B43D                 db    0
    .data:0040B43E                 db    0
    .data:0040B43F                 db    0
    .data:0040B440                 db    0
    .data:0040B441                 db    0
    .data:0040B442                 db    0
    .data:0040B443                 db    0
    .data:0040B444                 db    0
    .data:0040B445                 db    0
    .data:0040B446                 db    0
    .data:0040B447                 db    0
    .data:0040B448                 db    0
    .data:0040B449                 db    0
    .data:0040B44A                 db    0
    .data:0040B44B                 db    0
    .data:0040B44C                 db    0
    .data:0040B44D                 db    0
    .data:0040B44E                 db    0
    .data:0040B44F                 db    0
    .data:0040B450                 db    0
    .data:0040B451                 db    0
    .data:0040B452                 db    0
    .data:0040B453                 db    0
    .data:0040B454                 db    0
    .data:0040B455                 db    0
    .data:0040B456                 db    0
    .data:0040B457                 db    0
    .data:0040B458                 db    0
    .data:0040B459                 db    0
    .data:0040B45A                 db    0
    .data:0040B45B                 db    0
    .data:0040B45C                 db    0
    .data:0040B45D                 db    0
    .data:0040B45E                 db    0
    .data:0040B45F                 db    0
    .data:0040B460                 db    0
    .data:0040B461                 db    0
    .data:0040B462                 db    0
    .data:0040B463                 db    0
    .data:0040B464                 db    0
    .data:0040B465                 db    0
    .data:0040B466                 db    0
    .data:0040B467                 db    0
    .data:0040B468                 db    0
    .data:0040B469                 db    0
    .data:0040B46A                 db    0
    .data:0040B46B                 db    0
    .data:0040B46C                 db    0
    .data:0040B46D                 db    0
    .data:0040B46E                 db    0
    .data:0040B46F                 db    0
    .data:0040B470                 db    0
    .data:0040B471                 db    0
    .data:0040B472                 db    0
    .data:0040B473                 db    0
    .data:0040B474                 db    0
    .data:0040B475                 db    0
    .data:0040B476                 db    0
    .data:0040B477                 db    0
    .data:0040B478                 db    0
    .data:0040B479                 db    0
    .data:0040B47A                 db    0
    .data:0040B47B                 db    0
    .data:0040B47C                 db    0
    .data:0040B47D                 db    0
    .data:0040B47E                 db    0
    .data:0040B47F                 db    0
    .data:0040B480                 db    0
    .data:0040B481                 db    0
    .data:0040B482                 db    0
    .data:0040B483                 db    0
    .data:0040B484                 db    0
    .data:0040B485                 db    0
    .data:0040B486                 db    0
    .data:0040B487                 db    0
    .data:0040B488                 db    0
    .data:0040B489                 db    0
    .data:0040B48A                 db    0
    .data:0040B48B                 db    0
    .data:0040B48C                 db    0
    .data:0040B48D                 db    0
    .data:0040B48E                 db    0
    .data:0040B48F                 db    0
    .data:0040B490                 db    0
    .data:0040B491                 db    0
    .data:0040B492                 db    0
    .data:0040B493                 db    0
    .data:0040B494                 db    0
    .data:0040B495                 db    0
    .data:0040B496                 db    0
    .data:0040B497                 db    0
    .data:0040B498                 db    0
    .data:0040B499                 db    0
    .data:0040B49A                 db    0
    .data:0040B49B                 db    0
    .data:0040B49C                 db    0
    .data:0040B49D                 db    0
    .data:0040B49E                 db    0
    .data:0040B49F                 db    0
    .data:0040B4A0                 db    0
    .data:0040B4A1                 db    0
    .data:0040B4A2                 db    0
    .data:0040B4A3                 db    0
    .data:0040B4A4                 db    0
    .data:0040B4A5                 db    0
    .data:0040B4A6                 db    0
    .data:0040B4A7                 db    0
    .data:0040B4A8                 db    0
    .data:0040B4A9                 db    0
    .data:0040B4AA                 db    0
    .data:0040B4AB                 db    0
    .data:0040B4AC                 db    0
    .data:0040B4AD                 db    0
    .data:0040B4AE                 db    0
    .data:0040B4AF                 db    0
    .data:0040B4B0                 db    0
    .data:0040B4B1                 db    0
    .data:0040B4B2                 db    0
    .data:0040B4B3                 db    0
    .data:0040B4B4                 db    0
    .data:0040B4B5                 db    0
    .data:0040B4B6                 db    0
    .data:0040B4B7                 db    0
    .data:0040B4B8                 db    0
    .data:0040B4B9                 db    0
    .data:0040B4BA                 db    0
    .data:0040B4BB                 db    0
    .data:0040B4BC                 db    0
    .data:0040B4BD                 db    0
    .data:0040B4BE                 db    0
    .data:0040B4BF                 db    0
    .data:0040B4C0                 db    0
    .data:0040B4C1                 db    0
    .data:0040B4C2                 db    0
    .data:0040B4C3                 db    0
    .data:0040B4C4                 db    0
    .data:0040B4C5                 db    0
    .data:0040B4C6                 db    0
    .data:0040B4C7                 db    0
    .data:0040B4C8                 db    0
    .data:0040B4C9                 db    0
    .data:0040B4CA                 db    0
    .data:0040B4CB                 db    0
    .data:0040B4CC                 db    0
    .data:0040B4CD                 db    0
    .data:0040B4CE                 db    0
    .data:0040B4CF                 db    0
    .data:0040B4D0                 db    0
    .data:0040B4D1                 db    0
    .data:0040B4D2                 db    0
    .data:0040B4D3                 db    0
    .data:0040B4D4                 db    0
    .data:0040B4D5                 db    0
    .data:0040B4D6                 db    0
    .data:0040B4D7                 db    0
    .data:0040B4D8                 db    0
    .data:0040B4D9                 db    0
    .data:0040B4DA                 db    0
    .data:0040B4DB                 db    0
    .data:0040B4DC                 db    0
    .data:0040B4DD                 db    0
    .data:0040B4DE                 db    0
    .data:0040B4DF                 db    0
    .data:0040B4E0                 db    0
    .data:0040B4E1                 db    0
    .data:0040B4E2                 db    0
    .data:0040B4E3                 db    0
    .data:0040B4E4                 db    0
    .data:0040B4E5                 db    0
    .data:0040B4E6                 db    0
    .data:0040B4E7                 db    0
    .data:0040B4E8                 db    0
    .data:0040B4E9                 db    0
    .data:0040B4EA                 db    0
    .data:0040B4EB                 db    0
    .data:0040B4EC                 db    0
    .data:0040B4ED                 db    0
    .data:0040B4EE                 db    0
    .data:0040B4EF                 db    0
    .data:0040B4F0                 db    0
    .data:0040B4F1                 db    0
    .data:0040B4F2                 db    0
    .data:0040B4F3                 db    0
    .data:0040B4F4                 db    0
    .data:0040B4F5                 db    0
    .data:0040B4F6                 db    0
    .data:0040B4F7                 db    0
    .data:0040B4F8                 db    0
    .data:0040B4F9                 db    0
    .data:0040B4FA                 db    0
    .data:0040B4FB                 db    0
    .data:0040B4FC                 db    0
    .data:0040B4FD                 db    0
    .data:0040B4FE                 db    0
    .data:0040B4FF                 db    0
    .data:0040B500                 db    0
    .data:0040B501                 db    0
    .data:0040B502                 db    0
    .data:0040B503                 db    0
    .data:0040B504                 db    0
    .data:0040B505                 db    0
    .data:0040B506                 db    0
    .data:0040B507                 db    0
    .data:0040B508                 db    0
    .data:0040B509                 db    0
    .data:0040B50A                 db    0
    .data:0040B50B                 db    0
    .data:0040B50C                 db    0
    .data:0040B50D                 db    0
    .data:0040B50E                 db    0
    .data:0040B50F                 db    0
    .data:0040B510                 db    0
    .data:0040B511                 db    0
    .data:0040B512                 db    0
    .data:0040B513                 db    0
    .data:0040B514                 db    0
    .data:0040B515                 db    0
    .data:0040B516                 db    0
    .data:0040B517                 db    0
    .data:0040B518                 db    0
    .data:0040B519                 db    0
    .data:0040B51A                 db    0
    .data:0040B51B                 db    0
    .data:0040B51C                 db    0
    .data:0040B51D                 db    0
    .data:0040B51E                 db    0
    .data:0040B51F                 db    0
    .data:0040B520                 db    0
    .data:0040B521                 db    0
    .data:0040B522                 db    0
    .data:0040B523                 db    0
    .data:0040B524                 db    0
    .data:0040B525                 db    0
    .data:0040B526                 db    0
    .data:0040B527                 db    0
    .data:0040B528                 db    0
    .data:0040B529                 db    0
    .data:0040B52A                 db    0
    .data:0040B52B                 db    0
    .data:0040B52C                 db    0
    .data:0040B52D                 db    0
    .data:0040B52E                 db    0
    .data:0040B52F                 db    0
    .data:0040B530                 db    0
    .data:0040B531                 db    0
    .data:0040B532                 db    0
    .data:0040B533                 db    0
    .data:0040B534                 db    0
    .data:0040B535                 db    0
    .data:0040B536                 db    0
    .data:0040B537                 db    0
    .data:0040B538                 db    0
    .data:0040B539                 db    0
    .data:0040B53A                 db    0
    .data:0040B53B                 db    0
    .data:0040B53C                 db    0
    .data:0040B53D                 db    0
    .data:0040B53E                 db    0
    .data:0040B53F                 db    0
    .data:0040B540                 db    0
    .data:0040B541                 db    0
    .data:0040B542                 db    0
    .data:0040B543                 db    0
    .data:0040B544                 db    0
    .data:0040B545                 db    0
    .data:0040B546                 db    0
    .data:0040B547                 db    0
    .data:0040B548                 db    0
    .data:0040B549                 db    0
    .data:0040B54A                 db    0
    .data:0040B54B                 db    0
    .data:0040B54C                 db    0
    .data:0040B54D                 db    0
    .data:0040B54E                 db    0
    .data:0040B54F                 db    0
    .data:0040B550                 db    0
    .data:0040B551                 db    0
    .data:0040B552                 db    0
    .data:0040B553                 db    0
    .data:0040B554                 db    0
    .data:0040B555                 db    0
    .data:0040B556                 db    0
    .data:0040B557                 db    0
    .data:0040B558                 db    0
    .data:0040B559                 db    0
    .data:0040B55A                 db    0
    .data:0040B55B                 db    0
    .data:0040B55C                 db    0
    .data:0040B55D                 db    0
    .data:0040B55E                 db    0
    .data:0040B55F                 db    0
    .data:0040B560                 db    0
    .data:0040B561                 db    0
    .data:0040B562                 db    0
    .data:0040B563                 db    0
    .data:0040B564                 db    0
    .data:0040B565                 db    0
    .data:0040B566                 db    0
    .data:0040B567                 db    0
    .data:0040B568                 db    0
    .data:0040B569                 db    0
    .data:0040B56A                 db    0
    .data:0040B56B                 db    0
    .data:0040B56C                 db    0
    .data:0040B56D                 db    0
    .data:0040B56E                 db    0
    .data:0040B56F                 db    0
    .data:0040B570                 db    0
    .data:0040B571                 db    0
    .data:0040B572                 db    0
    .data:0040B573                 db    0
    .data:0040B574                 db    0
    .data:0040B575                 db    0
    .data:0040B576                 db    0
    .data:0040B577                 db    0
    .data:0040B578                 db    0
    .data:0040B579                 db    0
    .data:0040B57A                 db    0
    .data:0040B57B                 db    0
    .data:0040B57C                 db    0
    .data:0040B57D                 db    0
    .data:0040B57E                 db    0
    .data:0040B57F                 db    0
    .data:0040B580                 db    0
    .data:0040B581                 db    0
    .data:0040B582                 db    0
    .data:0040B583                 db    0
    .data:0040B584                 db    0
    .data:0040B585                 db    0
    .data:0040B586                 db    0
    .data:0040B587                 db    0
    .data:0040B588                 db    0
    .data:0040B589                 db    0
    .data:0040B58A                 db    0
    .data:0040B58B                 db    0
    .data:0040B58C                 db    0
    .data:0040B58D                 db    0
    .data:0040B58E                 db    0
    .data:0040B58F                 db    0
    .data:0040B590                 db    0
    .data:0040B591                 db    0
    .data:0040B592                 db    0
    .data:0040B593                 db    0
    .data:0040B594                 db    0
    .data:0040B595                 db    0
    .data:0040B596                 db    0
    .data:0040B597                 db    0
    .data:0040B598                 db    0
    .data:0040B599                 db    0
    .data:0040B59A                 db    0
    .data:0040B59B                 db    0
    .data:0040B59C                 db    0
    .data:0040B59D                 db    0
    .data:0040B59E                 db    0
    .data:0040B59F                 db    0
    .data:0040B5A0                 db    0
    .data:0040B5A1                 db    0
    .data:0040B5A2                 db    0
    .data:0040B5A3                 db    0
    .data:0040B5A4                 db    0
    .data:0040B5A5                 db    0
    .data:0040B5A6                 db    0
    .data:0040B5A7                 db    0
    .data:0040B5A8                 db    0
    .data:0040B5A9                 db    0
    .data:0040B5AA                 db    0
    .data:0040B5AB                 db    0
    .data:0040B5AC                 db    0
    .data:0040B5AD                 db    0
    .data:0040B5AE                 db    0
    .data:0040B5AF                 db    0
    .data:0040B5B0                 db    0
    .data:0040B5B1                 db    0
    .data:0040B5B2                 db    0
    .data:0040B5B3                 db    0
    .data:0040B5B4                 db    0
    .data:0040B5B5                 db    0
    .data:0040B5B6                 db    0
    .data:0040B5B7                 db    0
    .data:0040B5B8                 db    0
    .data:0040B5B9                 db    0
    .data:0040B5BA                 db    0
    .data:0040B5BB                 db    0
    .data:0040B5BC                 db    0
    .data:0040B5BD                 db    0
    .data:0040B5BE                 db    0
    .data:0040B5BF                 db    0
    .data:0040B5C0                 db    0
    .data:0040B5C1                 db    0
    .data:0040B5C2                 db    0
    .data:0040B5C3                 db    0
    .data:0040B5C4                 db    0
    .data:0040B5C5                 db    0
    .data:0040B5C6                 db    0
    .data:0040B5C7                 db    0
    .data:0040B5C8                 db    0
    .data:0040B5C9                 db    0
    .data:0040B5CA                 db    0
    .data:0040B5CB                 db    0
    .data:0040B5CC                 db    0
    .data:0040B5CD                 db    0
    .data:0040B5CE                 db    0
    .data:0040B5CF                 db    0
    .data:0040B5D0                 db    0
    .data:0040B5D1                 db    0
    .data:0040B5D2                 db    0
    .data:0040B5D3                 db    0
    .data:0040B5D4                 db    0
    .data:0040B5D5                 db    0
    .data:0040B5D6                 db    0
    .data:0040B5D7                 db    0
    .data:0040B5D8                 db    0
    .data:0040B5D9                 db    0
    .data:0040B5DA                 db    0
    .data:0040B5DB                 db    0
    .data:0040B5DC                 db    0
    .data:0040B5DD                 db    0
    .data:0040B5DE                 db    0
    .data:0040B5DF                 db    0
    .data:0040B5E0                 db    0
    .data:0040B5E1                 db    0
    .data:0040B5E2                 db    0
    .data:0040B5E3                 db    0
    .data:0040B5E4                 db    0
    .data:0040B5E5                 db    0
    .data:0040B5E6                 db    0
    .data:0040B5E7                 db    0
    .data:0040B5E8                 db    0
    .data:0040B5E9                 db    0
    .data:0040B5EA                 db    0
    .data:0040B5EB                 db    0
    .data:0040B5EC                 db    0
    .data:0040B5ED                 db    0
    .data:0040B5EE                 db    0
    .data:0040B5EF                 db    0
    .data:0040B5F0                 db    0
    .data:0040B5F1                 db    0
    .data:0040B5F2                 db    0
    .data:0040B5F3                 db    0
    .data:0040B5F4                 db    0
    .data:0040B5F5                 db    0
    .data:0040B5F6                 db    0
    .data:0040B5F7                 db    0
    .data:0040B5F8                 db    0
    .data:0040B5F9                 db    0
    .data:0040B5FA                 db    0
    .data:0040B5FB                 db    0
    .data:0040B5FC                 db    0
    .data:0040B5FD                 db    0
    .data:0040B5FE                 db    0
    .data:0040B5FF                 db    0
    .data:0040B600                 db    0
    .data:0040B601                 db    0
    .data:0040B602                 db    0
    .data:0040B603                 db    0
    .data:0040B604                 db    0
    .data:0040B605                 db    0
    .data:0040B606                 db    0
    .data:0040B607                 db    0
    .data:0040B608                 db    0
    .data:0040B609                 db    0
    .data:0040B60A                 db    0
    .data:0040B60B                 db    0
    .data:0040B60C                 db    0
    .data:0040B60D                 db    0
    .data:0040B60E                 db    0
    .data:0040B60F                 db    0
    .data:0040B610                 db    0
    .data:0040B611                 db    0
    .data:0040B612                 db    0
    .data:0040B613                 db    0
    .data:0040B614                 db    0
    .data:0040B615                 db    0
    .data:0040B616                 db    0
    .data:0040B617                 db    0
    .data:0040B618                 db    0
    .data:0040B619                 db    0
    .data:0040B61A                 db    0
    .data:0040B61B                 db    0
    .data:0040B61C                 db    0
    .data:0040B61D                 db    0
    .data:0040B61E                 db    0
    .data:0040B61F                 db    0
    .data:0040B620                 db    0
    .data:0040B621                 db    0
    .data:0040B622                 db    0
    .data:0040B623                 db    0
    .data:0040B624                 db    0
    .data:0040B625                 db    0
    .data:0040B626                 db    0
    .data:0040B627                 db    0
    .data:0040B628                 db    0
    .data:0040B629                 db    0
    .data:0040B62A                 db    0
    .data:0040B62B                 db    0
    .data:0040B62C                 db    0
    .data:0040B62D                 db    0
    .data:0040B62E                 db    0
    .data:0040B62F                 db    0
    .data:0040B630                 db    0
    .data:0040B631                 db    0
    .data:0040B632                 db    0
    .data:0040B633                 db    0
    .data:0040B634                 db    0
    .data:0040B635                 db    0
    .data:0040B636                 db    0
    .data:0040B637                 db    0
    .data:0040B638                 db    0
    .data:0040B639                 db    0
    .data:0040B63A                 db    0
    .data:0040B63B                 db    0
    .data:0040B63C                 db    0
    .data:0040B63D                 db    0
    .data:0040B63E                 db    0
    .data:0040B63F                 db    0
    .data:0040B640                 db    0
    .data:0040B641                 db    0
    .data:0040B642                 db    0
    .data:0040B643                 db    0
    .data:0040B644                 db    0
    .data:0040B645                 db    0
    .data:0040B646                 db    0
    .data:0040B647                 db    0
    .data:0040B648                 db    0
    .data:0040B649                 db    0
    .data:0040B64A                 db    0
    .data:0040B64B                 db    0
    .data:0040B64C                 db    0
    .data:0040B64D                 db    0
    .data:0040B64E                 db    0
    .data:0040B64F                 db    0
    .data:0040B650                 db    0
    .data:0040B651                 db    0
    .data:0040B652                 db    0
    .data:0040B653                 db    0
    .data:0040B654                 db    0
    .data:0040B655                 db    0
    .data:0040B656                 db    0
    .data:0040B657                 db    0
    .data:0040B658                 db    0
    .data:0040B659                 db    0
    .data:0040B65A                 db    0
    .data:0040B65B                 db    0
    .data:0040B65C                 db    0
    .data:0040B65D                 db    0
    .data:0040B65E                 db    0
    .data:0040B65F                 db    0
    .data:0040B660                 db    0
    .data:0040B661                 db    0
    .data:0040B662                 db    0
    .data:0040B663                 db    0
    .data:0040B664                 db    0
    .data:0040B665                 db    0
    .data:0040B666                 db    0
    .data:0040B667                 db    0
    .data:0040B668                 db    0
    .data:0040B669                 db    0
    .data:0040B66A                 db    0
    .data:0040B66B                 db    0
    .data:0040B66C                 db    0
    .data:0040B66D                 db    0
    .data:0040B66E                 db    0
    .data:0040B66F                 db    0
    .data:0040B670                 db    0
    .data:0040B671                 db    0
    .data:0040B672                 db    0
    .data:0040B673                 db    0
    .data:0040B674                 db    0
    .data:0040B675                 db    0
    .data:0040B676                 db    0
    .data:0040B677                 db    0
    .data:0040B678                 db    0
    .data:0040B679                 db    0
    .data:0040B67A                 db    0
    .data:0040B67B                 db    0
    .data:0040B67C                 db    0
    .data:0040B67D                 db    0
    .data:0040B67E                 db    0
    .data:0040B67F                 db    0
    .data:0040B680                 db    0
    .data:0040B681                 db    0
    .data:0040B682                 db    0
    .data:0040B683                 db    0
    .data:0040B684                 db    0
    .data:0040B685                 db    0
    .data:0040B686                 db    0
    .data:0040B687                 db    0
    .data:0040B688                 db    0
    .data:0040B689                 db    0
    .data:0040B68A                 db    0
    .data:0040B68B                 db    0
    .data:0040B68C                 db    0
    .data:0040B68D                 db    0
    .data:0040B68E                 db    0
    .data:0040B68F                 db    0
    .data:0040B690                 db    0
    .data:0040B691                 db    0
    .data:0040B692                 db    0
    .data:0040B693                 db    0
    .data:0040B694                 db    0
    .data:0040B695                 db    0
    .data:0040B696                 db    0
    .data:0040B697                 db    0
    .data:0040B698                 db    0
    .data:0040B699                 db    0
    .data:0040B69A                 db    0
    .data:0040B69B                 db    0
    .data:0040B69C                 db    0
    .data:0040B69D                 db    0
    .data:0040B69E                 db    0
    .data:0040B69F                 db    0
    .data:0040B6A0                 db    0
    .data:0040B6A1                 db    0
    .data:0040B6A2                 db    0
    .data:0040B6A3                 db    0
    .data:0040B6A4                 db    0
    .data:0040B6A5                 db    0
    .data:0040B6A6                 db    0
    .data:0040B6A7                 db    0
    .data:0040B6A8                 db    0
    .data:0040B6A9                 db    0
    .data:0040B6AA                 db    0
    .data:0040B6AB                 db    0
    .data:0040B6AC                 db    0
    .data:0040B6AD                 db    0
    .data:0040B6AE                 db    0
    .data:0040B6AF                 db    0
    .data:0040B6B0                 db    0
    .data:0040B6B1                 db    0
    .data:0040B6B2                 db    0
    .data:0040B6B3                 db    0
    .data:0040B6B4                 db    0
    .data:0040B6B5                 db    0
    .data:0040B6B6                 db    0
    .data:0040B6B7                 db    0
    .data:0040B6B8                 db    0
    .data:0040B6B9                 db    0
    .data:0040B6BA                 db    0
    .data:0040B6BB                 db    0
    .data:0040B6BC                 db    0
    .data:0040B6BD                 db    0
    .data:0040B6BE                 db    0
    .data:0040B6BF                 db    0
    .data:0040B6C0                 db    0
    .data:0040B6C1                 db    0
    .data:0040B6C2                 db    0
    .data:0040B6C3                 db    0
    .data:0040B6C4                 db    0
    .data:0040B6C5                 db    0
    .data:0040B6C6                 db    0
    .data:0040B6C7                 db    0
    .data:0040B6C8                 db    0
    .data:0040B6C9                 db    0
    .data:0040B6CA                 db    0
    .data:0040B6CB                 db    0
    .data:0040B6CC                 db    0
    .data:0040B6CD                 db    0
    .data:0040B6CE                 db    0
    .data:0040B6CF                 db    0
    .data:0040B6D0                 db    0
    .data:0040B6D1                 db    0
    .data:0040B6D2                 db    0
    .data:0040B6D3                 db    0
    .data:0040B6D4                 db    0
    .data:0040B6D5                 db    0
    .data:0040B6D6                 db    0
    .data:0040B6D7                 db    0
    .data:0040B6D8                 db    0
    .data:0040B6D9                 db    0
    .data:0040B6DA                 db    0
    .data:0040B6DB                 db    0
    .data:0040B6DC                 db    0
    .data:0040B6DD                 db    0
    .data:0040B6DE                 db    0
    .data:0040B6DF                 db    0
    .data:0040B6E0                 db    0
    .data:0040B6E1                 db    0
    .data:0040B6E2                 db    0
    .data:0040B6E3                 db    0
    .data:0040B6E4                 db    0
    .data:0040B6E5                 db    0
    .data:0040B6E6                 db    0
    .data:0040B6E7                 db    0
    .data:0040B6E8                 db    0
    .data:0040B6E9                 db    0
    .data:0040B6EA                 db    0
    .data:0040B6EB                 db    0
    .data:0040B6EC                 db    0
    .data:0040B6ED                 db    0
    .data:0040B6EE                 db    0
    .data:0040B6EF                 db    0
    .data:0040B6F0                 db    0
    .data:0040B6F1                 db    0
    .data:0040B6F2                 db    0
    .data:0040B6F3                 db    0
    .data:0040B6F4                 db    0
    .data:0040B6F5                 db    0
    .data:0040B6F6                 db    0
    .data:0040B6F7                 db    0
    .data:0040B6F8                 db    0
    .data:0040B6F9                 db    0
    .data:0040B6FA                 db    0
    .data:0040B6FB                 db    0
    .data:0040B6FC                 db    0
    .data:0040B6FD                 db    0
    .data:0040B6FE                 db    0
    .data:0040B6FF                 db    0
    .data:0040B700                 db    0
    .data:0040B701                 db    0
    .data:0040B702                 db    0
    .data:0040B703                 db    0
    .data:0040B704                 db    0
    .data:0040B705                 db    0
    .data:0040B706                 db    0
    .data:0040B707                 db    0
    .data:0040B708                 db    0
    .data:0040B709                 db    0
    .data:0040B70A                 db    0
    .data:0040B70B                 db    0
    .data:0040B70C                 db    0
    .data:0040B70D                 db    0
    .data:0040B70E                 db    0
    .data:0040B70F                 db    0
    .data:0040B710                 db    0
    .data:0040B711                 db    0
    .data:0040B712                 db    0
    .data:0040B713                 db    0
    .data:0040B714                 db    0
    .data:0040B715                 db    0
    .data:0040B716                 db    0
    .data:0040B717                 db    0
    .data:0040B718                 db    0
    .data:0040B719                 db    0
    .data:0040B71A                 db    0
    .data:0040B71B                 db    0
    .data:0040B71C                 db    0
    .data:0040B71D                 db    0
    .data:0040B71E                 db    0
    .data:0040B71F                 db    0
    .data:0040B720                 db    0
    .data:0040B721                 db    0
    .data:0040B722                 db    0
    .data:0040B723                 db    0
    .data:0040B724                 db    0
    .data:0040B725                 db    0
    .data:0040B726                 db    0
    .data:0040B727                 db    0
    .data:0040B728                 db    0
    .data:0040B729                 db    0
    .data:0040B72A                 db    0
    .data:0040B72B                 db    0
    .data:0040B72C                 db    0
    .data:0040B72D                 db    0
    .data:0040B72E                 db    0
    .data:0040B72F                 db    0
    .data:0040B730                 db    0
    .data:0040B731                 db    0
    .data:0040B732                 db    0
    .data:0040B733                 db    0
    .data:0040B734                 db    0
    .data:0040B735                 db    0
    .data:0040B736                 db    0
    .data:0040B737                 db    0
    .data:0040B738                 db    0
    .data:0040B739                 db    0
    .data:0040B73A                 db    0
    .data:0040B73B                 db    0
    .data:0040B73C                 db    0
    .data:0040B73D                 db    0
    .data:0040B73E                 db    0
    .data:0040B73F                 db    0
    .data:0040B740                 db    0
    .data:0040B741                 db    0
    .data:0040B742                 db    0
    .data:0040B743                 db    0
    .data:0040B744                 db    0
    .data:0040B745                 db    0
    .data:0040B746                 db    0
    .data:0040B747                 db    0
    .data:0040B748                 db    0
    .data:0040B749                 db    0
    .data:0040B74A                 db    0
    .data:0040B74B                 db    0
    .data:0040B74C                 db    0
    .data:0040B74D                 db    0
    .data:0040B74E                 db    0
    .data:0040B74F                 db    0
    .data:0040B750                 db    0
    .data:0040B751                 db    0
    .data:0040B752                 db    0
    .data:0040B753                 db    0
    .data:0040B754                 db    0
    .data:0040B755                 db    0
    .data:0040B756                 db    0
    .data:0040B757                 db    0
    .data:0040B758                 db    0
    .data:0040B759                 db    0
    .data:0040B75A                 db    0
    .data:0040B75B                 db    0
    .data:0040B75C                 db    0
    .data:0040B75D                 db    0
    .data:0040B75E                 db    0
    .data:0040B75F                 db    0
    .data:0040B760                 db    0
    .data:0040B761                 db    0
    .data:0040B762                 db    0
    .data:0040B763                 db    0
    .data:0040B764                 db    0
    .data:0040B765                 db    0
    .data:0040B766                 db    0
    .data:0040B767                 db    0
    .data:0040B768                 db    0
    .data:0040B769                 db    0
    .data:0040B76A                 db    0
    .data:0040B76B                 db    0
    .data:0040B76C                 db    0
    .data:0040B76D                 db    0
    .data:0040B76E                 db    0
    .data:0040B76F                 db    0
    .data:0040B770                 db    0
    .data:0040B771                 db    0
    .data:0040B772                 db    0
    .data:0040B773                 db    0
    .data:0040B774                 db    0
    .data:0040B775                 db    0
    .data:0040B776                 db    0
    .data:0040B777                 db    0
    .data:0040B778                 db    0
    .data:0040B779                 db    0
    .data:0040B77A                 db    0
    .data:0040B77B                 db    0
    .data:0040B77C                 db    0
    .data:0040B77D                 db    0
    .data:0040B77E                 db    0
    .data:0040B77F                 db    0
    .data:0040B780                 db    0
    .data:0040B781                 db    0
    .data:0040B782                 db    0
    .data:0040B783                 db    0
    .data:0040B784                 db    0
    .data:0040B785                 db    0
    .data:0040B786                 db    0
    .data:0040B787                 db    0
    .data:0040B788                 db    0
    .data:0040B789                 db    0
    .data:0040B78A                 db    0
    .data:0040B78B                 db    0
    .data:0040B78C                 db    0
    .data:0040B78D                 db    0
    .data:0040B78E                 db    0
    .data:0040B78F                 db    0
    .data:0040B790                 db    0
    .data:0040B791                 db    0
    .data:0040B792                 db    0
    .data:0040B793                 db    0
    .data:0040B794                 db    0
    .data:0040B795                 db    0
    .data:0040B796                 db    0
    .data:0040B797                 db    0
    .data:0040B798                 db    0
    .data:0040B799                 db    0
    .data:0040B79A                 db    0
    .data:0040B79B                 db    0
    .data:0040B79C                 db    0
    .data:0040B79D                 db    0
    .data:0040B79E                 db    0
    .data:0040B79F                 db    0
    .data:0040B7A0                 db    0
    .data:0040B7A1                 db    0
    .data:0040B7A2                 db    0
    .data:0040B7A3                 db    0
    .data:0040B7A4                 db    0
    .data:0040B7A5                 db    0
    .data:0040B7A6                 db    0
    .data:0040B7A7                 db    0
    .data:0040B7A8                 db    0
    .data:0040B7A9                 db    0
    .data:0040B7AA                 db    0
    .data:0040B7AB                 db    0
    .data:0040B7AC                 db    0
    .data:0040B7AD                 db    0
    .data:0040B7AE                 db    0
    .data:0040B7AF                 db    0
    .data:0040B7B0                 db    0
    .data:0040B7B1                 db    0
    .data:0040B7B2                 db    0
    .data:0040B7B3                 db    0
    .data:0040B7B4                 db    0
    .data:0040B7B5                 db    0
    .data:0040B7B6                 db    0
    .data:0040B7B7                 db    0
    .data:0040B7B8                 db    0
    .data:0040B7B9                 db    0
    .data:0040B7BA                 db    0
    .data:0040B7BB                 db    0
    .data:0040B7BC                 db    0
    .data:0040B7BD                 db    0
    .data:0040B7BE                 db    0
    .data:0040B7BF                 db    0
    
    .data:0040A100 unk_40A100      db 0A3h ; ú             ; DATA XREF: _main+1Ao
    .data:0040A101                 db  3Fh ; ?
    .data:0040A102                 db 0ACh ; ¼
    .data:0040A103                 db 0FDh ; ²
    .data:0040A104                 db 0BAh ; ¦
    .data:0040A105                 db 0B4h ; ¦
    .data:0040A106                 db  28h ; (
    .data:0040A107                 db  1Bh
    .data:0040A108                 db 0C5h ; +
    .data:0040A109                 db 0B6h ; ¦
    .data:0040A10A                 db 0E5h ; s
    .data:0040A10B                 db    8
    .data:0040A10C                 db  9Eh ; P
    .data:0040A10D                 db    3
    .data:0040A10E                 db  4Fh ; O
    .data:0040A10F                 db  72h ; r
    .data:0040A110                 db 0CBh ; -
    .data:0040A111                 db 0A8h ; ¿
    .data:0040A112                 db  0Ch
    .data:0040A113                 db  0Fh
    .data:0040A114                 db  5Ah ; Z
    .data:0040A115                 db 0B3h ; ¦
    .data:0040A116                 db  25h ; %
    .data:0040A117                 db  8Fh ; Å
    .data:0040A118                 db  99h ; Ö
    .data:0040A119                 db  45h ; E
    .data:0040A11A                 db 0B4h ; ¦
    .data:0040A11B                 db 0D5h ; +
    .data:0040A11C                 db  10h
    .data:0040A11D                 db  97h ; ù
    .data:0040A11E                 db    6
    .data:0040A11F                 db  6Eh ; n
    .data:0040A120                 db  10h
    .data:0040A121                 db  73h ; s
    .data:0040A122                 db  27h ; '
    .data:0040A123                 db  1Dh
    .data:0040A124                 db  37h ; 7
    .data:0040A125                 db  96h ; û
    .data:0040A126                 db  5Ah ; Z
    .data:0040A127                 db  6Dh ; m
    .data:0040A128                 db 0B8h ; +
    .data:0040A129                 db 0A0h ; á
    .data:0040A12A                 db 0CCh ; ¦
    .data:0040A12B                 db 0CCh ; ¦
    .data:0040A12C                 db  76h ; v
    .data:0040A12D                 db 0D5h ; +
    .data:0040A12E                 db 0CFh ; -
    .data:0040A12F                 db 0A4h ; ñ
    .data:0040A130                 db  7Eh ; ~
    .data:0040A131                 db 0D3h ; +
    .data:0040A132                 db 0CFh ; -
    .data:0040A133                 db  92h ; Æ
    .data:0040A134                 db  72h ; r
    .data:0040A135                 db 0D5h ; +
    .data:0040A136                 db  6Bh ; k
    .data:0040A137                 db  39h ; 9
    .data:0040A138                 db  79h ; y
    .data:0040A139                 db  16h
    .data:0040A13A                 db 0F5h ; )
    .data:0040A13B                 db  14h
    .data:0040A13C                 db 0A0h ; á
    .data:0040A13D                 db  24h ; $
    .data:0040A13E                 db  3Fh ; ?
    .data:0040A13F                 db 0DAh ; +
    .data:0040A140                 db  6Ah ; j
    .data:0040A141                 db 0C5h ; +
    .data:0040A142                 db 0C0h ; +
    .data:0040A143                 db  68h ; h
    .data:0040A144                 db  96h ; û
    .data:0040A145                 db  18h
    .data:0040A146                 db  4Fh ; O
    .data:0040A147                 db  18h
    .data:0040A148                 db 0CDh ; -
    .data:0040A149                 db  9Fh ; ƒ
    .data:0040A14A                 db  16h
    .data:0040A14B                 db  60h ; `
    .data:0040A14C                 db 0F5h ; )
    .data:0040A14D                 db  22h ; "
    .data:0040A14E                 db 0B5h ; ¦
    .data:0040A14F                 db  5Ah ; Z
    .data:0040A150                 db  9Ah ; Ü
    .data:0040A151                 db  27h ; '
    .data:0040A152                 db  41h ; A
    .data:0040A153                 db  0Ah
    .data:0040A154                 db 0B2h ; ¦
    .data:0040A155                 db  11h
    .data:0040A156                 db    7
    .data:0040A157                 db  61h ; a
    .data:0040A158                 db  98h ; ÿ
    .data:0040A159                 db 0F3h ; =
    .data:0040A15A                 db 0A2h ; ó
    .data:0040A15B                 db 0CBh ; -
    .data:0040A15C                 db    2
    .data:0040A15D                 db 0FEh ; ¦
    .data:0040A15E                 db  42h ; B
    .data:0040A15F                 db  3Fh ; ?
    .data:0040A160                 db  62h ; b
    .data:0040A161                 db 0B6h ; ¦
    .data:0040A162                 db  9Eh ; P
    .data:0040A163                 db  92h ; Æ
    .data:0040A164                 db 0E0h ; a
    .data:0040A165                 db  42h ; B
    .data:0040A166                 db  89h ; ë
    .data:0040A167                 db 0ACh ; ¼
    .data:0040A168                 db  73h ; s
    .data:0040A169                 db  11h
    .data:0040A16A                 db  1Fh
    .data:0040A16B                 db  41h ; A
    .data:0040A16C                 db 0A9h ; ¬
    .data:0040A16D                 db  25h ; %
    .data:0040A16E                 db 0ECh ; 8
    .data:0040A16F                 db  27h ; '
    .data:0040A170                 db 0C6h ; ¦
    .data:0040A171                 db 0B2h ; ¦
    .data:0040A172                 db  29h ; )
    .data:0040A173                 db  84h ; ä
    .data:0040A174                 db 0BAh ; ¦
    .data:0040A175                 db 0F3h ; =
    .data:0040A176                 db  45h ; E
    .data:0040A177                 db  62h ; b
    .data:0040A178                 db    6
    .data:0040A179                 db  54h ; T
    .data:0040A17A                 db  7Bh ; {
    .data:0040A17B                 db 0E0h ; a
    .data:0040A17C                 db 0AFh ; »
    .data:0040A17D                 db 0DBh ; ¦
    .data:0040A17E                 db  1Fh
    .data:0040A17F                 db  0Ah
    .data:0040A180                 db  46h ; F
    .data:0040A181                 db 0F8h ; °
    .data:0040A182                 db 0C6h ; ¦
    .data:0040A183                 db  21h ; !
    .data:0040A184                 db 0A2h ; ó
    .data:0040A185                 db  13h
    .data:0040A186                 db 0B2h ; ¦
    .data:0040A187                 db 0CEh ; +
    .data:0040A188                 db  56h ; V
    .data:0040A189                 db  83h ; â
    .data:0040A18A                 db  69h ; i
    .data:0040A18B                 db  8Eh ; Ä
    .data:0040A18C                 db  87h ; ç
    .data:0040A18D                 db  5Bh ; [
    .data:0040A18E                 db  73h ; s
    .data:0040A18F                 db  4Ah ; J
    .data:0040A190                 db 0A0h ; á
    .data:0040A191                 db  9Bh ; ¢
    .data:0040A192                 db 0C5h ; +
    .data:0040A193                 db  77h ; w
    .data:0040A194                 db  11h
    .data:0040A195                 db  46h ; F
    .data:0040A196                 db 0A4h ; ñ
    .data:0040A197                 db  2Dh ; -
    .data:0040A198                 db  94h ; ö
    .data:0040A199                 db  61h ; a
    .data:0040A19A                 db 0A4h ; ñ
    .data:0040A19B                 db  86h ; å
    .data:0040A19C                 db  26h ; &
    .data:0040A19D                 db  5Bh ; [
    .data:0040A19E                 db    9
    .data:0040A19F                 db  41h ; A
    .data:0040A1A0                 db  2Ah ; *
    .data:0040A1A1                 db 0F0h ; =
    .data:0040A1A2                 db  27h ; '
    .data:0040A1A3                 db  70h ; p
    .data:0040A1A4                 db 0E9h ; T
    .data:0040A1A5                 db 0FAh ; ·
    .data:0040A1A6                 db  98h ; ÿ
    .data:0040A1A7                 db  3Ah ; :
    .data:0040A1A8                 db  6Dh ; m
    .data:0040A1A9                 db  3Bh ; ;
    .data:0040A1AA                 db 0CAh ; -
    .data:0040A1AB                 db  68h ; h
    .data:0040A1AC                 db  50h ; P
    .data:0040A1AD                 db 0A2h ; ó
    .data:0040A1AE                 db 0CEh ; +
    .data:0040A1AF                 db 0D2h ; -
    .data:0040A1B0                 db  9Ch ; £
    .data:0040A1B1                 db 0A2h ; ó
    .data:0040A1B2                 db  76h ; v
    .data:0040A1B3                 db 0E6h ; µ
    .data:0040A1B4                 db 0C7h ; ¦
    .data:0040A1B5                 db 0F4h ; (
    .data:0040A1B6                 db    5
    .data:0040A1B7                 db 0C3h ; +
    .data:0040A1B8                 db 0D9h ; +
    .data:0040A1B9                 db 0F8h ; °
    .data:0040A1BA                 db  24h ; $
    .data:0040A1BB                 db  48h ; H
    .data:0040A1BC                 db 0EAh ; O
    .data:0040A1BD                 db  17h
    .data:0040A1BE                 db  58h ; X
    .data:0040A1BF                 db  7Ch ; |
    .data:0040A1C0                 db 0E4h ; S
    .data:0040A1C1                 db 0BBh ; +
    .data:0040A1C2                 db  90h ; É
    .data:0040A1C3                 db  2Fh ; /
    .data:0040A1C4                 db  4Ch ; L
    .data:0040A1C5                 db  5Eh ; ^
    .data:0040A1C6                 db 0AAh ; ¬
    .data:0040A1C7                 db  3Ah ; :
    .data:0040A1C8                 db 0EFh ; n
    .data:0040A1C9                 db  2Fh ; /
    .data:0040A1CA                 db  7Bh ; {
    .data:0040A1CB                 db  41h ; A
    .data:0040A1CC                 db 0C8h ; +
    .data:0040A1CD                 db  4Dh ; M
    .data:0040A1CE                 db  29h ; )
    .data:0040A1CF                 db 0E3h ; p
    .data:0040A1D0                 db  75h ; u
    .data:0040A1D1                 db 0BBh ; +
    .data:0040A1D2                 db 0FCh ; n
    .data:0040A1D3                 db  2Dh ; -
    .data:0040A1D4                 db 0F2h ; =
    .data:0040A1D5                 db 0DCh ; _
    .data:0040A1D6                 db 0E6h ; µ
    .data:0040A1D7                 db 0BDh ; +
    .data:0040A1D8                 db 0AFh ; »
    .data:0040A1D9                 db  2Ch ; ,
    .data:0040A1DA                 db  66h ; f
    .data:0040A1DB                 db    3
    .data:0040A1DC                 db    2
    .data:0040A1DD                 db  1Bh
    .data:0040A1DE                 db  88h ; ê
    .data:0040A1DF                 db  68h ; h
    .data:0040A1E0                 db  91h ; æ
    .data:0040A1E1                 db 0A6h ; ª
    .data:0040A1E2                 db 0B5h ; ¦
    .data:0040A1E3                 db  5Fh ; _
    .data:0040A1E4                 db 0DFh ; ¯
    .data:0040A1E5                 db  97h ; ù
    .data:0040A1E6                 db 0FFh
    .data:0040A1E7                 db  31h ; 1
    .data:0040A1E8                 db 0D8h ; +
    .data:0040A1E9                 db  8Ah ; è
    .data:0040A1EA                 db  1Ah
    .data:0040A1EB                 db 0E1h ; ß
    .data:0040A1EC                 db  3Ah ; :
    .data:0040A1ED                 db  22h ; "
    .data:0040A1EE                 db 0CFh ; -
    .data:0040A1EF                 db 0B2h ; ¦
    .data:0040A1F0                 db  26h ; &
    .data:0040A1F1                 db  90h ; É
    .data:0040A1F2                 db 0FFh
    .data:0040A1F3                 db  75h ; u
    .data:0040A1F4                 db 0ADh ; ¡
    .data:0040A1F5                 db 0D1h ; -
    .data:0040A1F6                 db 0F3h ; =
    .data:0040A1F7                 db 0C6h ; ¦
    .data:0040A1F8                 db  35h ; 5
    .data:0040A1F9                 db  40h ; @
    .data:0040A1FA                 db  39h ; 9
    .data:0040A1FB                 db  69h ; i
    .data:0040A1FC                 db 0F7h ; ˜
    .data:0040A1FD                 db  66h ; f
    .data:0040A1FE                 db  3Bh ; ;
    .data:0040A1FF                 db    0
    
    .data:0040BFC0 ; const WCHAR szPassword
    .data:0040BFC0 szPassword      dw 0                    ; DATA XREF: sub_401080+32o
    .data:0040BFC0                                         ; sub_401160+32o ...
    .data:0040BFC2                 db    0
    .data:0040BFC3                 db    0
    .data:0040BFC4                 db    0
    .data:0040BFC5                 db    0
    .data:0040BFC6                 db    0
    .data:0040BFC7                 db    0
    .data:0040BFC8                 db    0
    .data:0040BFC9                 db    0
    .data:0040BFCA                 db    0
    .data:0040BFCB                 db    0
    .data:0040BFCC                 db    0
    .data:0040BFCD                 db    0
    .data:0040BFCE                 db    0
    .data:0040BFCF                 db    0
    .data:0040BFD0                 db    0
    .data:0040BFD1                 db    0
    .data:0040BFD2                 db    0
    .data:0040BFD3                 db    0
    .data:0040BFD4                 db    0
    .data:0040BFD5                 db    0
    .data:0040BFD6                 db    0
    .data:0040BFD7                 db    0
    .data:0040BFD8                 db    0
    .data:0040BFD9                 db    0
    .data:0040BFDA                 db    0
    .data:0040BFDB                 db    0
    .data:0040BFDC                 db    0
    .data:0040BFDD                 db    0
    .data:0040BFDE                 db    0
    .data:0040BFDF                 db    0
    .data:0040BFE0                 db    0
    .data:0040BFE1                 db    0
    .data:0040BFE2                 db    0
    .data:0040BFE3                 db    0
    .data:0040BFE4                 db    0
    .data:0040BFE5                 db    0
    .data:0040BFE6                 db    0
    .data:0040BFE7                 db    0
    .data:0040BFE8                 db    0
    .data:0040BFE9                 db    0
    .data:0040BFEA                 db    0
    .data:0040BFEB                 db    0
    .data:0040BFEC                 db    0
    .data:0040BFED                 db    0
    .data:0040BFEE                 db    0
    .data:0040BFEF                 db    0
    .data:0040BFF0                 db    0
    .data:0040BFF1                 db    0
    .data:0040BFF2                 db    0
    .data:0040BFF3                 db    0
    .data:0040BFF4                 db    0
    .data:0040BFF5                 db    0
    .data:0040BFF6                 db    0
    .data:0040BFF7                 db    0
    .data:0040BFF8                 db    0
    .data:0040BFF9                 db    0
    .data:0040BFFA                 db    0
    .data:0040BFFB                 db    0
    .data:0040BFFC                 db    0
    .data:0040BFFD                 db    0
    .data:0040BFFE                 db    0
    .data:0040BFFF                 db    0
    .data:0040C000                 db    ? ;
    .data:0040C001                 db    ? ;
    .data:0040C002                 db    ? ;
    .data:0040C003                 db    ? ;
    .data:0040C004                 db    ? ;
    .data:0040C005                 db    ? ;
    .data:0040C006                 db    ? ;
    .data:0040C007                 db    ? ;
    .data:0040C008                 db    ? ;
    .data:0040C009                 db    ? ;
    .data:0040C00A                 db    ? ;
    .data:0040C00B                 db    ? ;
    .data:0040C00C                 db    ? ;
    .data:0040C00D                 db    ? ;
    .data:0040C00E                 db    ? ;
    .data:0040C00F                 db    ? ;
    .data:0040C010                 db    ? ;
    .data:0040C011                 db    ? ;
    .data:0040C012                 db    ? ;
    .data:0040C013                 db    ? ;
    .data:0040C014                 db    ? ;
    .data:0040C015                 db    ? ;
    .data:0040C016                 db    ? ;
    .data:0040C017                 db    ? ;
    .data:0040C018                 db    ? ;
    .data:0040C019                 db    ? ;
    .data:0040C01A                 db    ? ;
    .data:0040C01B                 db    ? ;
    .data:0040C01C                 db    ? ;
    .data:0040C01D                 db    ? ;
    .data:0040C01E                 db    ? ;
    .data:0040C01F                 db    ? ;
    .data:0040C020                 db    ? ;
    .data:0040C021                 db    ? ;
    .data:0040C022                 db    ? ;
    .data:0040C023                 db    ? ;
    .data:0040C024                 db    ? ;
    .data:0040C025                 db    ? ;
    .data:0040C026                 db    ? ;
    .data:0040C027                 db    ? ;
    .data:0040C028                 db    ? ;
    .data:0040C029                 db    ? ;
    .data:0040C02A                 db    ? ;
    .data:0040C02B                 db    ? ;
    .data:0040C02C                 db    ? ;
    .data:0040C02D                 db    ? ;
    .data:0040C02E                 db    ? ;
    .data:0040C02F                 db    ? ;
    .data:0040C030                 db    ? ;
    .data:0040C031                 db    ? ;
    .data:0040C032                 db    ? ;
    .data:0040C033                 db    ? ;
    .data:0040C034                 db    ? ;
    .data:0040C035                 db    ? ;
    .data:0040C036                 db    ? ;
    .data:0040C037                 db    ? ;
    .data:0040C038                 db    ? ;
    .data:0040C039                 db    ? ;
    .data:0040C03A                 db    ? ;
    .data:0040C03B                 db    ? ;
    .data:0040C03C                 db    ? ;
    .data:0040C03D                 db    ? ;
    .data:0040C03E                 db    ? ;
    .data:0040C03F                 db    ? ;
    .data:0040C040                 db    ? ;
    .data:0040C041                 db    ? ;
    .data:0040C042                 db    ? ;
    .data:0040C043                 db    ? ;
    .data:0040C044                 db    ? ;
    .data:0040C045                 db    ? ;
    .data:0040C046                 db    ? ;
    .data:0040C047                 db    ? ;
    .data:0040C048                 db    ? ;
    .data:0040C049                 db    ? ;
    .data:0040C04A                 db    ? ;
    .data:0040C04B                 db    ? ;
    .data:0040C04C                 db    ? ;
    .data:0040C04D                 db    ? ;
    .data:0040C04E                 db    ? ;
    .data:0040C04F                 db    ? ;
    .data:0040C050                 db    ? ;
    .data:0040C051                 db    ? ;
    .data:0040C052                 db    ? ;
    .data:0040C053                 db    ? ;
    .data:0040C054                 db    ? ;
    .data:0040C055                 db    ? ;
    .data:0040C056                 db    ? ;
    .data:0040C057                 db    ? ;
    .data:0040C058                 db    ? ;
    .data:0040C059                 db    ? ;
    .data:0040C05A                 db    ? ;
    .data:0040C05B                 db    ? ;
    .data:0040C05C                 db    ? ;
    .data:0040C05D                 db    ? ;
    .data:0040C05E                 db    ? ;
    .data:0040C05F                 db    ? ;
    .data:0040C060                 db    ? ;
    .data:0040C061                 db    ? ;
    .data:0040C062                 db    ? ;
    .data:0040C063                 db    ? ;
    .data:0040C064                 db    ? ;
    .data:0040C065                 db    ? ;
    .data:0040C066                 db    ? ;
    .data:0040C067                 db    ? ;
    .data:0040C068                 db    ? ;
    .data:0040C069                 db    ? ;
    .data:0040C06A                 db    ? ;
    .data:0040C06B                 db    ? ;
    .data:0040C06C                 db    ? ;
    .data:0040C06D                 db    ? ;
    .data:0040C06E                 db    ? ;
    .data:0040C06F                 db    ? ;
    .data:0040C070                 db    ? ;
    .data:0040C071                 db    ? ;
    .data:0040C072                 db    ? ;
    .data:0040C073                 db    ? ;
    .data:0040C074                 db    ? ;
    .data:0040C075                 db    ? ;
    .data:0040C076                 db    ? ;
    .data:0040C077                 db    ? ;
    .data:0040C078                 db    ? ;
    .data:0040C079                 db    ? ;
    .data:0040C07A                 db    ? ;
    .data:0040C07B                 db    ? ;
    .data:0040C07C                 db    ? ;
    .data:0040C07D                 db    ? ;
    .data:0040C07E                 db    ? ;
    .data:0040C07F                 db    ? ;
    .data:0040C080                 db    ? ;
    .data:0040C081                 db    ? ;
    .data:0040C082                 db    ? ;
    .data:0040C083                 db    ? ;
    .data:0040C084                 db    ? ;
    .data:0040C085                 db    ? ;
    .data:0040C086                 db    ? ;
    .data:0040C087                 db    ? ;
    .data:0040C088                 db    ? ;
    .data:0040C089                 db    ? ;
    .data:0040C08A                 db    ? ;
    .data:0040C08B                 db    ? ;
    .data:0040C08C                 db    ? ;
    .data:0040C08D                 db    ? ;
    .data:0040C08E                 db    ? ;
    .data:0040C08F                 db    ? ;
    .data:0040C090                 db    ? ;
    .data:0040C091                 db    ? ;
    .data:0040C092                 db    ? ;
    .data:0040C093                 db    ? ;
    .data:0040C094                 db    ? ;
    .data:0040C095                 db    ? ;
    .data:0040C096                 db    ? ;
    .data:0040C097                 db    ? ;
    .data:0040C098                 db    ? ;
    .data:0040C099                 db    ? ;
    .data:0040C09A                 db    ? ;
    .data:0040C09B                 db    ? ;
    .data:0040C09C                 db    ? ;
    .data:0040C09D                 db    ? ;
    .data:0040C09E                 db    ? ;
    .data:0040C09F                 db    ? ;
    .data:0040C0A0                 db    ? ;
    .data:0040C0A1                 db    ? ;
    .data:0040C0A2                 db    ? ;
    .data:0040C0A3                 db    ? ;
    .data:0040C0A4                 db    ? ;
    .data:0040C0A5                 db    ? ;
    .data:0040C0A6                 db    ? ;
    .data:0040C0A7                 db    ? ;
    .data:0040C0A8                 db    ? ;
    .data:0040C0A9                 db    ? ;
    .data:0040C0AA                 db    ? ;
    .data:0040C0AB                 db    ? ;
    .data:0040C0AC                 db    ? ;
    .data:0040C0AD                 db    ? ;
    .data:0040C0AE                 db    ? ;
    .data:0040C0AF                 db    ? ;
    .data:0040C0B0                 db    ? ;
    .data:0040C0B1                 db    ? ;
    .data:0040C0B2                 db    ? ;
    .data:0040C0B3                 db    ? ;
    .data:0040C0B4                 db    ? ;
    .data:0040C0B5                 db    ? ;
    .data:0040C0B6                 db    ? ;
    .data:0040C0B7                 db    ? ;
    .data:0040C0B8                 db    ? ;
    .data:0040C0B9                 db    ? ;
    .data:0040C0BA                 db    ? ;
    .data:0040C0BB                 db    ? ;
    .data:0040C0BC                 db    ? ;
    .data:0040C0BD                 db    ? ;
    .data:0040C0BE                 db    ? ;
    .data:0040C0BF                 db    ? ;
    .data:0040C0C0                 db    ? ;
    .data:0040C0C1                 db    ? ;
    .data:0040C0C2                 db    ? ;
    .data:0040C0C3                 db    ? ;
    .data:0040C0C4                 db    ? ;
    .data:0040C0C5                 db    ? ;
    .data:0040C0C6                 db    ? ;
    .data:0040C0C7                 db    ? ;
    .data:0040C0C8                 db    ? ;
    .data:0040C0C9                 db    ? ;
    .data:0040C0CA                 db    ? ;
    .data:0040C0CB                 db    ? ;
    .data:0040C0CC                 db    ? ;
    .data:0040C0CD                 db    ? ;
    .data:0040C0CE                 db    ? ;
    .data:0040C0CF                 db    ? ;
    .data:0040C0D0                 db    ? ;
    .data:0040C0D1                 db    ? ;
    .data:0040C0D2                 db    ? ;
    .data:0040C0D3                 db    ? ;
    .data:0040C0D4                 db    ? ;
    .data:0040C0D5                 db    ? ;
    .data:0040C0D6                 db    ? ;
    .data:0040C0D7                 db    ? ;
    .data:0040C0D8                 db    ? ;
    .data:0040C0D9                 db    ? ;
    .data:0040C0DA                 db    ? ;
    .data:0040C0DB                 db    ? ;
    .data:0040C0DC                 db    ? ;
    .data:0040C0DD                 db    ? ;
    .data:0040C0DE                 db    ? ;
    .data:0040C0DF                 db    ? ;
    .data:0040C0E0                 db    ? ;
    .data:0040C0E1                 db    ? ;
    .data:0040C0E2                 db    ? ;
    .data:0040C0E3                 db    ? ;
    .data:0040C0E4                 db    ? ;
    .data:0040C0E5                 db    ? ;
    .data:0040C0E6                 db    ? ;
    .data:0040C0E7                 db    ? ;
    .data:0040C0E8                 db    ? ;
    .data:0040C0E9                 db    ? ;
    .data:0040C0EA                 db    ? ;
    .data:0040C0EB                 db    ? ;
    .data:0040C0EC                 db    ? ;
    .data:0040C0ED                 db    ? ;
    .data:0040C0EE                 db    ? ;
    .data:0040C0EF                 db    ? ;
    .data:0040C0F0                 db    ? ;
    .data:0040C0F1                 db    ? ;
    .data:0040C0F2                 db    ? ;
    .data:0040C0F3                 db    ? ;
    .data:0040C0F4                 db    ? ;
    .data:0040C0F5                 db    ? ;
    .data:0040C0F6                 db    ? ;
    .data:0040C0F7                 db    ? ;
    .data:0040C0F8                 db    ? ;
    .data:0040C0F9                 db    ? ;
    .data:0040C0FA                 db    ? ;
    .data:0040C0FB                 db    ? ;
    .data:0040C0FC                 db    ? ;
    .data:0040C0FD                 db    ? ;
    .data:0040C0FE                 db    ? ;
    .data:0040C0FF                 db    ? ;
    .data:0040C100                 db    ? ;
    .data:0040C101                 db    ? ;
    .data:0040C102                 db    ? ;
    .data:0040C103                 db    ? ;
    .data:0040C104                 db    ? ;
    .data:0040C105                 db    ? ;
    .data:0040C106                 db    ? ;
    .data:0040C107                 db    ? ;
    .data:0040C108                 db    ? ;
    .data:0040C109                 db    ? ;
    .data:0040C10A                 db    ? ;
    .data:0040C10B                 db    ? ;
    .data:0040C10C                 db    ? ;
    .data:0040C10D                 db    ? ;
    .data:0040C10E                 db    ? ;
    .data:0040C10F                 db    ? ;
    .data:0040C110                 db    ? ;
    .data:0040C111                 db    ? ;
    .data:0040C112                 db    ? ;
    .data:0040C113                 db    ? ;
    .data:0040C114                 db    ? ;
    .data:0040C115                 db    ? ;
    .data:0040C116                 db    ? ;
    .data:0040C117                 db    ? ;
    .data:0040C118                 db    ? ;
    .data:0040C119                 db    ? ;
    .data:0040C11A                 db    ? ;
    .data:0040C11B                 db    ? ;
    .data:0040C11C                 db    ? ;
    .data:0040C11D                 db    ? ;
    .data:0040C11E                 db    ? ;
    .data:0040C11F                 db    ? ;
    .data:0040C120                 db    ? ;
    .data:0040C121                 db    ? ;
    .data:0040C122                 db    ? ;
    .data:0040C123                 db    ? ;
    .data:0040C124                 db    ? ;
    .data:0040C125                 db    ? ;
    .data:0040C126                 db    ? ;
    .data:0040C127                 db    ? ;
    .data:0040C128                 db    ? ;
    .data:0040C129                 db    ? ;
    .data:0040C12A                 db    ? ;
    .data:0040C12B                 db    ? ;
    .data:0040C12C                 db    ? ;
    .data:0040C12D                 db    ? ;
    .data:0040C12E                 db    ? ;
    .data:0040C12F                 db    ? ;
    .data:0040C130                 db    ? ;
    .data:0040C131                 db    ? ;
    .data:0040C132                 db    ? ;
    .data:0040C133                 db    ? ;
    .data:0040C134                 db    ? ;
    .data:0040C135                 db    ? ;
    .data:0040C136                 db    ? ;
    .data:0040C137                 db    ? ;
    .data:0040C138                 db    ? ;
    .data:0040C139                 db    ? ;
    .data:0040C13A                 db    ? ;
    .data:0040C13B                 db    ? ;
    .data:0040C13C                 db    ? ;
    .data:0040C13D                 db    ? ;
    .data:0040C13E                 db    ? ;
    .data:0040C13F                 db    ? ;
    .data:0040C140                 db    ? ;
    .data:0040C141                 db    ? ;
    .data:0040C142                 db    ? ;
    .data:0040C143                 db    ? ;
    .data:0040C144                 db    ? ;
    .data:0040C145                 db    ? ;
    .data:0040C146                 db    ? ;
    .data:0040C147                 db    ? ;
    .data:0040C148                 db    ? ;
    .data:0040C149                 db    ? ;
    .data:0040C14A                 db    ? ;
    .data:0040C14B                 db    ? ;
    .data:0040C14C                 db    ? ;
    .data:0040C14D                 db    ? ;
    .data:0040C14E                 db    ? ;
    .data:0040C14F                 db    ? ;
    .data:0040C150                 db    ? ;
    .data:0040C151                 db    ? ;
    .data:0040C152                 db    ? ;
    .data:0040C153                 db    ? ;
    .data:0040C154                 db    ? ;
    .data:0040C155                 db    ? ;
    .data:0040C156                 db    ? ;
    .data:0040C157                 db    ? ;
    .data:0040C158                 db    ? ;
    .data:0040C159                 db    ? ;
    .data:0040C15A                 db    ? ;
    .data:0040C15B                 db    ? ;
    .data:0040C15C                 db    ? ;
    .data:0040C15D                 db    ? ;
    .data:0040C15E                 db    ? ;
    .data:0040C15F                 db    ? ;
    .data:0040C160                 db    ? ;
    .data:0040C161                 db    ? ;
    .data:0040C162                 db    ? ;
    .data:0040C163                 db    ? ;
    .data:0040C164                 db    ? ;
    .data:0040C165                 db    ? ;
    .data:0040C166                 db    ? ;
    .data:0040C167                 db    ? ;
    .data:0040C168                 db    ? ;
    .data:0040C169                 db    ? ;
    .data:0040C16A                 db    ? ;
    .data:0040C16B                 db    ? ;
    .data:0040C16C                 db    ? ;
    .data:0040C16D                 db    ? ;
    .data:0040C16E                 db    ? ;
    .data:0040C16F                 db    ? ;
    .data:0040C170                 db    ? ;
    .data:0040C171                 db    ? ;
    .data:0040C172                 db    ? ;
    .data:0040C173                 db    ? ;
    .data:0040C174                 db    ? ;
    .data:0040C175                 db    ? ;
    .data:0040C176                 db    ? ;
    .data:0040C177                 db    ? ;
    .data:0040C178                 db    ? ;
    .data:0040C179                 db    ? ;
    .data:0040C17A                 db    ? ;
    .data:0040C17B                 db    ? ;
    .data:0040C17C                 db    ? ;
    .data:0040C17D                 db    ? ;
    .data:0040C17E                 db    ? ;
    .data:0040C17F                 db    ? ;
    .data:0040C180                 db    ? ;
    .data:0040C181                 db    ? ;
    .data:0040C182                 db    ? ;
    .data:0040C183                 db    ? ;
    .data:0040C184                 db    ? ;
    .data:0040C185                 db    ? ;
    .data:0040C186                 db    ? ;
    .data:0040C187                 db    ? ;
    .data:0040C188                 db    ? ;
    .data:0040C189                 db    ? ;
    .data:0040C18A                 db    ? ;
    .data:0040C18B                 db    ? ;
    .data:0040C18C                 db    ? ;
    .data:0040C18D                 db    ? ;
    .data:0040C18E                 db    ? ;
    .data:0040C18F                 db    ? ;
    .data:0040C190                 db    ? ;
    .data:0040C191                 db    ? ;
    .data:0040C192                 db    ? ;
    .data:0040C193                 db    ? ;
    .data:0040C194                 db    ? ;
    .data:0040C195                 db    ? ;
    .data:0040C196                 db    ? ;
    .data:0040C197                 db    ? ;
    .data:0040C198                 db    ? ;
    .data:0040C199                 db    ? ;
    .data:0040C19A                 db    ? ;
    .data:0040C19B                 db    ? ;
    .data:0040C19C                 db    ? ;
    .data:0040C19D                 db    ? ;
    .data:0040C19E                 db    ? ;
    .data:0040C19F                 db    ? ;
    .data:0040C1A0                 db    ? ;
    .data:0040C1A1                 db    ? ;
    .data:0040C1A2                 db    ? ;
    .data:0040C1A3                 db    ? ;
    .data:0040C1A4                 db    ? ;
    .data:0040C1A5                 db    ? ;
    .data:0040C1A6                 db    ? ;
    .data:0040C1A7                 db    ? ;
    .data:0040C1A8                 db    ? ;
    .data:0040C1A9                 db    ? ;
    .data:0040C1AA                 db    ? ;
    .data:0040C1AB                 db    ? ;
    .data:0040C1AC                 db    ? ;
    .data:0040C1AD                 db    ? ;
    .data:0040C1AE                 db    ? ;
    .data:0040C1AF                 db    ? ;
    .data:0040C1B0                 db    ? ;
    .data:0040C1B1                 db    ? ;
    .data:0040C1B2                 db    ? ;
    .data:0040C1B3                 db    ? ;
    .data:0040C1B4                 db    ? ;
    .data:0040C1B5                 db    ? ;
    .data:0040C1B6                 db    ? ;
    .data:0040C1B7                 db    ? ;
    .data:0040C1B8                 db    ? ;
    .data:0040C1B9                 db    ? ;
    .data:0040C1BA                 db    ? ;
    .data:0040C1BB                 db    ? ;
    .data:0040C1BC                 db    ? ;
    .data:0040C1BD                 db    ? ;
    .data:0040C1BE                 db    ? ;
    .data:0040C1BF                 db    ? ;
    
    .data:0040A200 unk_40A200      db 0D7h ; +             ; DATA XREF: _main+2Co
    .data:0040A201                 db  33h ; 3
    .data:0040A202                 db  31h ; 1
    .data:0040A203                 db 0D8h ; +
    .data:0040A204                 db  40h ; @
    .data:0040A205                 db 0F2h ; =
    .data:0040A206                 db  4Eh ; N
    .data:0040A207                 db  14h
    .data:0040A208                 db 0E9h ; T
    .data:0040A209                 db  2Dh ; -
    .data:0040A20A                 db 0A7h ; º
    .data:0040A20B                 db 0E6h ; µ
    .data:0040A20C                 db 0EFh ; n
    .data:0040A20D                 db  5Ah ; Z
    .data:0040A20E                 db  36h ; 6
    .data:0040A20F                 db  89h ; ë
    .data:0040A210                 db  72h ; r
    .data:0040A211                 db 0FCh ; n
    .data:0040A212                 db  89h ; ë
    .data:0040A213                 db 0C1h ; -
    .data:0040A214                 db  94h ; ö
    .data:0040A215                 db  1Bh
    .data:0040A216                 db  74h ; t
    .data:0040A217                 db  1Eh
    .data:0040A218                 db 0CAh ; -
    .data:0040A219                 db 0AFh ; »
    .data:0040A21A                 db 0D2h ; -
    .data:0040A21B                 db  7Fh ; 
    .data:0040A21C                 db  5Ah ; Z
    .data:0040A21D                 db  6Eh ; n
    .data:0040A21E                 db  32h ; 2
    .data:0040A21F                 db  66h ; f
    .data:0040A220                 db  82h ; é
    .data:0040A221                 db  99h ; Ö
    .data:0040A222                 db 0FDh ; ²
    .data:0040A223                 db 0C4h ; -
    .data:0040A224                 db  0Eh
    .data:0040A225                 db 0B0h ; ¦
    .data:0040A226                 db  75h ; u
    .data:0040A227                 db  6Bh ; k
    .data:0040A228                 db  27h ; '
    .data:0040A229                 db 0ABh ; ½
    .data:0040A22A                 db  89h ; ë
    .data:0040A22B                 db 0BDh ; +
    .data:0040A22C                 db  3Bh ; ;
    .data:0040A22D                 db 0A3h ; ú
    .data:0040A22E                 db  70h ; p
    .data:0040A22F                 db 0C7h ; ¦
    .data:0040A230                 db 0DDh ; ¦
    .data:0040A231                 db  90h ; É
    .data:0040A232                 db    9
    .data:0040A233                 db  66h ; f
    .data:0040A234                 db  4Ah ; J
    .data:0040A235                 db 0F3h ; =
    .data:0040A236                 db 0D9h ; +
    .data:0040A237                 db  95h ; ò
    .data:0040A238                 db  98h ; ÿ
    .data:0040A239                 db 0A6h ; ª
    .data:0040A23A                 db  48h ; H
    .data:0040A23B                 db 0A1h ; í
    .data:0040A23C                 db  3Bh ; ;
    .data:0040A23D                 db  1Ah
    .data:0040A23E                 db 0D5h ; +
    .data:0040A23F                 db 0B4h ; ¦
    .data:0040A240                 db 0D0h ; -
    .data:0040A241                 db 0C4h ; -
    .data:0040A242                 db 0FCh ; n
    .data:0040A243                 db  24h ; $
    .data:0040A244                 db 0ECh ; 8
    .data:0040A245                 db    8
    .data:0040A246                 db  74h ; t
    .data:0040A247                 db  56h ; V
    .data:0040A248                 db 0D7h ; +
    .data:0040A249                 db  4Ch ; L
    .data:0040A24A                 db  88h ; ê
    .data:0040A24B                 db 0ACh ; ¼
    .data:0040A24C                 db 0F0h ; =
    .data:0040A24D                 db  21h ; !
    .data:0040A24E                 db 0B9h ; ¦
    .data:0040A24F                 db  5Eh ; ^
    .data:0040A250                 db 0B1h ; ¦
    .data:0040A251                 db  10h
    .data:0040A252                 db 0CFh ; -
    .data:0040A253                 db  0Ch
    .data:0040A254                 db  73h ; s
    .data:0040A255                 db  8Ah ; è
    .data:0040A256                 db  34h ; 4
    .data:0040A257                 db  17h
    .data:0040A258                 db    7
    .data:0040A259                 db  87h ; ç
    .data:0040A25A                 db  94h ; ö
    .data:0040A25B                 db 0FAh ; ·
    .data:0040A25C                 db 0B2h ; ¦
    .data:0040A25D                 db 0C5h ; +
    .data:0040A25E                 db  8Fh ; Å
    .data:0040A25F                 db 0C9h ; +
    .data:0040A260                 db  6Ch ; l
    .data:0040A261                 db 0E2h ; G
    .data:0040A262                 db 0D0h ; -
    .data:0040A263                 db 0D8h ; +
    .data:0040A264                 db  3Ah ; :
    .data:0040A265                 db 0A2h ; ó
    .data:0040A266                 db  9Eh ; P
    .data:0040A267                 db  64h ; d
    .data:0040A268                 db    8
    .data:0040A269                 db  8Ah ; è
    .data:0040A26A                 db  53h ; S
    .data:0040A26B                 db  4Ah ; J
    .data:0040A26C                 db  69h ; i
    .data:0040A26D                 db 0E7h ; t
    .data:0040A26E                 db  6Eh ; n
    .data:0040A26F                 db  54h ; T
    .data:0040A270                 db  7Ah ; z
    .data:0040A271                 db 0F5h ; )
    .data:0040A272                 db  95h ; ò
    .data:0040A273                 db  2Fh ; /
    .data:0040A274                 db 0BAh ; ¦
    .data:0040A275                 db    3
    .data:0040A276                 db  3Dh ; =
    .data:0040A277                 db  9Bh ; ¢
    .data:0040A278                 db 0C5h ; +
    .data:0040A279                 db 0E6h ; µ
    .data:0040A27A                 db  99h ; Ö
    .data:0040A27B                 db  0Fh
    .data:0040A27C                 db 0DBh ; ¦
    .data:0040A27D                 db  42h ; B
    .data:0040A27E                 db  78h ; x
    .data:0040A27F                 db 0DEh ; ¦
    .data:0040A280                 db 0EFh ; n
    .data:0040A281                 db  12h
    .data:0040A282                 db    5
    .data:0040A283                 db  57h ; W
    .data:0040A284                 db 0FEh ; ¦
    .data:0040A285                 db  95h ; ò
    .data:0040A286                 db  35h ; 5
    .data:0040A287                 db 0BAh ; ¦
    .data:0040A288                 db  89h ; ë
    .data:0040A289                 db  17h
    .data:0040A28A                 db 0FAh ; ·
    .data:0040A28B                 db    2
    .data:0040A28C                 db    1
    .data:0040A28D                 db    2
    .data:0040A28E                 db  12h
    .data:0040A28F                 db 0C3h ; +
    .data:0040A290                 db  8Ah ; è
    .data:0040A291                 db 0ECh ; 8
    .data:0040A292                 db  72h ; r
    .data:0040A293                 db 0A0h ; á
    .data:0040A294                 db 0CDh ; -
    .data:0040A295                 db  73h ; s
    .data:0040A296                 db 0CEh ; +
    .data:0040A297                 db  33h ; 3
    .data:0040A298                 db 0C6h ; ¦
    .data:0040A299                 db  90h ; É
    .data:0040A29A                 db  19h
    .data:0040A29B                 db  32h ; 2
    .data:0040A29C                 db  53h ; S
    .data:0040A29D                 db 0D2h ; -
    .data:0040A29E                 db 0FAh ; ·
    .data:0040A29F                 db 0EEh ; e
    .data:0040A2A0                 db 0E3h ; p
    .data:0040A2A1                 db  8Eh ; Ä
    .data:0040A2A2                 db  44h ; D
    .data:0040A2A3                 db  4Ch ; L
    .data:0040A2A4                 db  0Dh
    .data:0040A2A5                 db  7Bh ; {
    .data:0040A2A6                 db  2Ch ; ,
    .data:0040A2A7                 db  54h ; T
    .data:0040A2A8                 db  6Fh ; o
    .data:0040A2A9                 db  54h ; T
    .data:0040A2AA                 db 0F3h ; =
    .data:0040A2AB                 db  14h
    .data:0040A2AC                 db  19h
    .data:0040A2AD                 db  6Eh ; n
    .data:0040A2AE                 db 0C8h ; +
    .data:0040A2AF                 db 0D9h ; +
    .data:0040A2B0                 db  77h ; w
    .data:0040A2B1                 db  55h ; U
    .data:0040A2B2                 db 0E6h ; µ
    .data:0040A2B3                 db    7
    .data:0040A2B4                 db 0DCh ; _
    .data:0040A2B5                 db 0E6h ; µ
    .data:0040A2B6                 db  67h ; g
    .data:0040A2B7                 db  81h ; ü
    .data:0040A2B8                 db  3Fh ; ?
    .data:0040A2B9                 db  7Fh ; 
    .data:0040A2BA                 db 0BAh ; ¦
    .data:0040A2BB                 db  90h ; É
    .data:0040A2BC                 db  3Dh ; =
    .data:0040A2BD                 db  2Fh ; /
    .data:0040A2BE                 db 0B2h ; ¦
    .data:0040A2BF                 db  16h
    .data:0040A2C0                 db  77h ; w
    .data:0040A2C1                 db  81h ; ü
    .data:0040A2C2                 db  1Fh
    .data:0040A2C3                 db 0F7h ; ˜
    .data:0040A2C4                 db 0E2h ; G
    .data:0040A2C5                 db  55h ; U
    .data:0040A2C6                 db 0E6h ; µ
    .data:0040A2C7                 db 0BDh ; +
    .data:0040A2C8                 db  90h ; É
    .data:0040A2C9                 db 0DAh ; +
    .data:0040A2CA                 db  19h
    .data:0040A2CB                 db  94h ; ö
    .data:0040A2CC                 db  96h ; û
    .data:0040A2CD                 db  9Eh ; P
    .data:0040A2CE                 db 0DEh ; ¦
    .data:0040A2CF                 db  5Bh ; [
    .data:0040A2D0                 db  98h ; ÿ
    .data:0040A2D1                 db  45h ; E
    .data:0040A2D2                 db  55h ; U
    .data:0040A2D3                 db 0D7h ; +
    .data:0040A2D4                 db  9Fh ; ƒ
    .data:0040A2D5                 db  5Ch ; \
    .data:0040A2D6                 db  2Ah ; *
    .data:0040A2D7                 db  3Dh ; =
    .data:0040A2D8                 db  2Ah ; *
    .data:0040A2D9                 db  67h ; g
    .data:0040A2DA                 db  89h ; ë
    .data:0040A2DB                 db  25h ; %
    .data:0040A2DC                 db  3Fh ; ?
    .data:0040A2DD                 db  84h ; ä
    .data:0040A2DE                 db  39h ; 9
    .data:0040A2DF                 db  9Eh ; P
    .data:0040A2E0                 db 0E5h ; s
    .data:0040A2E1                 db  58h ; X
    .data:0040A2E2                 db 0E9h ; T
    .data:0040A2E3                 db 0FAh ; ·
    .data:0040A2E4                 db 0B8h ; +
    .data:0040A2E5                 db  1Ch
    .data:0040A2E6                 db  1Bh
    .data:0040A2E7                 db 0F6h ; ÷
    .data:0040A2E8                 db  8Bh ; ï
    .data:0040A2E9                 db  74h ; t
    .data:0040A2EA                 db  26h ; &
    .data:0040A2EB                 db  6Bh ; k
    .data:0040A2EC                 db 0E0h ; a
    .data:0040A2ED                 db 0F7h ; ˜
    .data:0040A2EE                 db 0C0h ; +
    .data:0040A2EF                 db  9Ch ; £
    .data:0040A2F0                 db  8Ch ; î
    .data:0040A2F1                 db    4
    .data:0040A2F2                 db  83h ; â
    .data:0040A2F3                 db 0E2h ; G
    .data:0040A2F4                 db 0CDh ; -
    .data:0040A2F5                 db 0C7h ; ¦
    .data:0040A2F6                 db 0DDh ; ¦
    .data:0040A2F7                 db 0B2h ; ¦
    .data:0040A2F8                 db 0C4h ; -
    .data:0040A2F9                 db  2Ch ; ,
    .data:0040A2FA                 db 0F5h ; )
    .data:0040A2FB                 db 0C4h ; -
    .data:0040A2FC                 db    5
    .data:0040A2FD                 db  71h ; q
    .data:0040A2FE                 db 0D1h ; -
    .data:0040A2FF                 db    0
    
    .data:0040A308 unk_40A308      db  81h ; ü             ; DATA XREF: _main+3Eo
    .data:0040A309                 db 0D5h ; +
    .data:0040A30A                 db 0FFh
    .data:0040A30B                 db 0ECh ; 8
    .data:0040A30C                 db  20h
    .data:0040A30D                 db  23h ; #
    .data:0040A30E                 db 0EFh ; n
    .data:0040A30F                 db  35h ; 5
    .data:0040A310                 db  4Ch ; L
    .data:0040A311                 db 0AAh ; ¬
    .data:0040A312                 db 0C7h ; ¦
    .data:0040A313                 db 0B9h ; ¦
    .data:0040A314                 db  7Ch ; |
    .data:0040A315                 db 0D5h ; +
    .data:0040A316                 db 0DDh ; ¦
    .data:0040A317                 db 0D7h ; +
    .data:0040A318                 db  65h ; e
    .data:0040A319                 db 0B4h ; ¦
    .data:0040A31A                 db 0D0h ; -
    .data:0040A31B                 db 0D6h ; +
    .data:0040A31C                 db  6Bh ; k
    .data:0040A31D                 db 0D8h ; +
    .data:0040A31E                 db 0D7h ; +
    .data:0040A31F                 db 0C9h ; +
    .data:0040A320                 db  65h ; e
    .data:0040A321                 db 0B4h ; ¦
    .data:0040A322                 db 0D0h ; -
    .data:0040A323                 db 0D7h ; +
    .data:0040A324                 db  74h ; t
    .data:0040A325                 db 0E4h ; S
    .data:0040A326                 db 0DAh ; +
    .data:0040A327                 db 0D4h ; +
    .data:0040A328                 db  65h ; e
    .data:0040A329                 db 0E2h ; G
    .data:0040A32A                 db 0D0h ; -
    .data:0040A32B                 db 0C7h ; ¦
    .data:0040A32C                 db  6Eh ; n
    .data:0040A32D                 db 0D9h ; +
    .data:0040A32E                 db 0DBh ; ¦
    .data:0040A32F                 db 0D8h ; +
    .data:0040A330                 db  59h ; Y
    .data:0040A331                 db 0D5h ; +
    .data:0040A332                 db 0DFh ; ¯
    .data:0040A333                 db 0D6h ; +
    .data:0040A334                 db  78h ; x
    .data:0040A335                 db 0E6h ; µ
    .data:0040A336                 db 0CAh ; -
    .data:0040A337                 db  9Dh ; ¥
    .data:0040A338                 db  3Ch ; <
    .data:0040A339                 db 0A1h ; í
    .data:0040A33A                 db 0A1h ; í
    .data:0040A33B                 db  92h ; Æ
    .data:0040A33C                 db  79h ; y
    .data:0040A33D                 db 0D4h ; +
    .data:0040A33E                 db 0D1h ; -
    .data:0040A33F                 db  64h ; d
    .data:0040A340                 db    6
    .data:0040A341                 db 0EAh ; O
    .data:0040A342                 db 0F2h ; =
    .data:0040A343                 db 0D8h ; +
    .data:0040A344                 db    9
    .data:0040A345                 db 0EDh ; f
    .data:0040A346                 db  41h ; A
    .data:0040A347                 db  5Eh ; ^
    .data:0040A348                 db 0ACh ; ¼
    .data:0040A349                 db 0C5h ; +
    .data:0040A34A                 db  54h ; T
    .data:0040A34B                 db  26h ; &
    .data:0040A34C                 db  6Ah ; j
    .data:0040A34D                 db  27h ; '
    .data:0040A34E                 db 0F1h ; ±
    .data:0040A34F                 db  6Dh ; m
    .data:0040A350                 db    7
    .data:0040A351                 db 0FBh ; v
    .data:0040A352                 db  5Ch ; \
    .data:0040A353                 db 0ADh ; ¡
    .data:0040A354                 db  9Eh ; P
    .data:0040A355                 db  27h ; '
    .data:0040A356                 db  16h
    .data:0040A357                 db  96h ; û
    .data:0040A358                 db  3Bh ; ;
    .data:0040A359                 db 0FAh ; ·
    .data:0040A35A                 db  16h
    .data:0040A35B                 db 0C4h ; -
    .data:0040A35C                 db  44h ; D
    .data:0040A35D                 db  40h ; @
    .data:0040A35E                 db  39h ; 9
    .data:0040A35F                 db  38h ; 8
    .data:0040A360                 db 0B1h ; ¦
    .data:0040A361                 db 0F7h ; ˜
    .data:0040A362                 db  0Eh
    .data:0040A363                 db 0CBh ; -
    .data:0040A364                 db 0ABh ; ½
    .data:0040A365                 db 0BFh ; +
    .data:0040A366                 db 0C0h ; +
    .data:0040A367                 db  35h ; 5
    .data:0040A368                 db  1Ah
    .data:0040A369                 db  6Fh ; o
    .data:0040A36A                 db 0C7h ; ¦
    .data:0040A36B                 db  53h ; S
    .data:0040A36C                 db 0D7h ; +
    .data:0040A36D                 db  5Fh ; _
    .data:0040A36E                 db 0A2h ; ó
    .data:0040A36F                 db  45h ; E
    .data:0040A370                 db  6Eh ; n
    .data:0040A371                 db 0FAh ; ·
    .data:0040A372                 db 0B8h ; +
    .data:0040A373                 db  99h ; Ö
    .data:0040A374                 db  9Eh ; P
    .data:0040A375                 db 0FBh ; v
    .data:0040A376                 db 0B4h ; ¦
    .data:0040A377                 db  95h ; ò
    .data:0040A378                 db  1Dh
    .data:0040A379                 db  79h ; y
    .data:0040A37A                 db 0E3h ; p
    .data:0040A37B                 db 0D0h ; -
    .data:0040A37C                 db  47h ; G
    .data:0040A37D                 db  28h ; (
    .data:0040A37E                 db    5
    .data:0040A37F                 db 0B8h ; +
    .data:0040A380                 db  30h ; 0
    .data:0040A381                 db  7Dh ; }
    .data:0040A382                 db 0F7h ; ˜
    .data:0040A383                 db  35h ; 5
    .data:0040A384                 db 0C7h ; ¦
    .data:0040A385                 db  82h ; é
    .data:0040A386                 db  47h ; G
    .data:0040A387                 db  6Ah ; j
    .data:0040A388                 db  0Fh
    .data:0040A389                 db  16h
    .data:0040A38A                 db  7Fh ; 
    .data:0040A38B                 db  79h ; y
    .data:0040A38C                 db    4
    .data:0040A38D                 db 0E5h ; s
    .data:0040A38E                 db  47h ; G
    .data:0040A38F                 db  9Ah ; Ü
    .data:0040A390                 db  48h ; H
    .data:0040A391                 db 0E0h ; a
    .data:0040A392                 db 0A7h ; º
    .data:0040A393                 db  7Dh ; }
    .data:0040A394                 db 0A7h ; º
    .data:0040A395                 db  66h ; f
    .data:0040A396                 db 0FEh ; ¦
    .data:0040A397                 db  52h ; R
    .data:0040A398                 db 0F8h ; °
    .data:0040A399                 db 0F1h ; ±
    .data:0040A39A                 db  12h
    .data:0040A39B                 db 0D6h ; +
    .data:0040A39C                 db  11h
    .data:0040A39D                 db  99h ; Ö
    .data:0040A39E                 db 0A7h ; º
    .data:0040A39F                 db  61h ; a
    .data:0040A3A0                 db  33h ; 3
    .data:0040A3A1                 db  83h ; â
    .data:0040A3A2                 db 0B2h ; ¦
    .data:0040A3A3                 db  2Ah ; *
    .data:0040A3A4                 db  3Eh ; >
    .data:0040A3A5                 db  3Ah ; :
    .data:0040A3A6                 db 0E7h ; t
    .data:0040A3A7                 db 0E2h ; G
    .data:0040A3A8                 db  7Eh ; ~
    .data:0040A3A9                 db 0FFh
    .data:0040A3AA                 db 0C9h ; +
    .data:0040A3AB                 db  51h ; Q
    .data:0040A3AC                 db 0DDh ; ¦
    .data:0040A3AD                 db  8Ch ; î
    .data:0040A3AE                 db  8Eh ; Ä
    .data:0040A3AF                 db    7
    .data:0040A3B0                 db 0E8h ; F
    .data:0040A3B1                 db 0CFh ; -
    .data:0040A3B2                 db  60h ; `
    .data:0040A3B3                 db 0D7h ; +
    .data:0040A3B4                 db  5Ch ; \
    .data:0040A3B5                 db  21h ; !
    .data:0040A3B6                 db 0DCh ; _
    .data:0040A3B7                 db 0BAh ; ¦
    .data:0040A3B8                 db 0A3h ; ú
    .data:0040A3B9                 db  84h ; ä
    .data:0040A3BA                 db 0DCh ; _
    .data:0040A3BB                 db  3Dh ; =
    .data:0040A3BC                 db  11h
    .data:0040A3BD                 db  5Eh ; ^
    .data:0040A3BE                 db 0DFh ; ¯
    .data:0040A3BF                 db  94h ; ö
    .data:0040A3C0                 db  30h ; 0
    .data:0040A3C1                 db 0C9h ; +
    .data:0040A3C2                 db  26h ; &
    .data:0040A3C3                 db  16h
    .data:0040A3C4                 db 0F1h ; ±
    .data:0040A3C5                 db 0DDh ; ¦
    .data:0040A3C6                 db  5Ch ; \
    .data:0040A3C7                 db  15h
    .data:0040A3C8                 db 0A1h ; í
    .data:0040A3C9                 db  28h ; (
    .data:0040A3CA                 db 0D5h ; +
    .data:0040A3CB                 db  6Ch ; l
    .data:0040A3CC                 db 0D9h ; +
    .data:0040A3CD                 db  18h
    .data:0040A3CE                 db  48h ; H
    .data:0040A3CF                 db 0B7h ; +
    .data:0040A3D0                 db  69h ; i
    .data:0040A3D1                 db  9Fh ; ƒ
    .data:0040A3D2                 db 0F9h ; ·
    .data:0040A3D3                 db  7Ch ; |
    .data:0040A3D4                 db  60h ; `
    .data:0040A3D5                 db 0E0h ; a
    .data:0040A3D6                 db  57h ; W
    .data:0040A3D7                 db 0D2h ; -
    .data:0040A3D8                 db 0B5h ; ¦
    .data:0040A3D9                 db  86h ; å
    .data:0040A3DA                 db 0E7h ; t
    .data:0040A3DB                 db 0BCh ; +
    .data:0040A3DC                 db 0BEh ; +
    .data:0040A3DD                 db 0B6h ; ¦
    .data:0040A3DE                 db  90h ; É
    .data:0040A3DF                 db 0CAh ; -
    .data:0040A3E0                 db  62h ; b
    .data:0040A3E1                 db 0BEh ; +
    .data:0040A3E2                 db  9Dh ; ¥
    .data:0040A3E3                 db 0B5h ; ¦
    .data:0040A3E4                 db 0C7h ; ¦
    .data:0040A3E5                 db  5Bh ; [
    .data:0040A3E6                 db 0FFh
    .data:0040A3E7                 db  8Eh ; Ä
    .data:0040A3E8                 db  72h ; r
    .data:0040A3E9                 db 0BDh ; +
    .data:0040A3EA                 db 0B8h ; +
    .data:0040A3EB                 db  2Bh ; +
    .data:0040A3EC                 db 0EEh ; e
    .data:0040A3ED                 db  41h ; A
    .data:0040A3EE                 db 0E9h ; T
    .data:0040A3EF                 db  6Ch ; l
    .data:0040A3F0                 db 0A4h ; ñ
    .data:0040A3F1                 db 0DCh ; _
    .data:0040A3F2                 db  73h ; s
    .data:0040A3F3                 db  14h
    .data:0040A3F4                 db 0DBh ; ¦
    .data:0040A3F5                 db 0CBh ; -
    .data:0040A3F6                 db  1Bh
    .data:0040A3F7                 db 0AEh ; «
    .data:0040A3F8                 db  8Ch ; î
    .data:0040A3F9                 db  80h ; Ç
    .data:0040A3FA                 db  38h ; 8
    .data:0040A3FB                 db 0E1h ; ß
    .data:0040A3FC                 db  13h
    .data:0040A3FD                 db 0D4h ; +
    .data:0040A3FE                 db 0C0h ; +
    .data:0040A3FF                 db  8Dh ; ì
    .data:0040A400                 db  46h ; F
    .data:0040A401                 db  0Bh
    .data:0040A402                 db 0C8h ; +
    .data:0040A403                 db  1Bh
    .data:0040A404                 db  2Ch ; ,
    .data:0040A405                 db  11h
    .data:0040A406                 db  51h ; Q
    .data:0040A407                 db    0
    
    .data:0040B7C0 ; wchar_t szLocalFile
    .data:0040B7C0 szLocalFile     dw 0                    ; DATA XREF: _main+39o
    .data:0040B7C0                                         ; _main+81o
    .data:0040B7C2                 db    0
    .data:0040B7C3                 db    0
    .data:0040B7C4                 db    0
    .data:0040B7C5                 db    0
    .data:0040B7C6                 db    0
    .data:0040B7C7                 db    0
    .data:0040B7C8                 db    0
    .data:0040B7C9                 db    0
    .data:0040B7CA                 db    0
    .data:0040B7CB                 db    0
    .data:0040B7CC                 db    0
    .data:0040B7CD                 db    0
    .data:0040B7CE                 db    0
    .data:0040B7CF                 db    0
    .data:0040B7D0                 db    0
    .data:0040B7D1                 db    0
    .data:0040B7D2                 db    0
    .data:0040B7D3                 db    0
    .data:0040B7D4                 db    0
    .data:0040B7D5                 db    0
    .data:0040B7D6                 db    0
    .data:0040B7D7                 db    0
    .data:0040B7D8                 db    0
    .data:0040B7D9                 db    0
    .data:0040B7DA                 db    0
    .data:0040B7DB                 db    0
    .data:0040B7DC                 db    0
    .data:0040B7DD                 db    0
    .data:0040B7DE                 db    0
    .data:0040B7DF                 db    0
    .data:0040B7E0                 db    0
    .data:0040B7E1                 db    0
    .data:0040B7E2                 db    0
    .data:0040B7E3                 db    0
    .data:0040B7E4                 db    0
    .data:0040B7E5                 db    0
    .data:0040B7E6                 db    0
    .data:0040B7E7                 db    0
    .data:0040B7E8                 db    0
    .data:0040B7E9                 db    0
    .data:0040B7EA                 db    0
    .data:0040B7EB                 db    0
    .data:0040B7EC                 db    0
    .data:0040B7ED                 db    0
    .data:0040B7EE                 db    0
    .data:0040B7EF                 db    0
    .data:0040B7F0                 db    0
    .data:0040B7F1                 db    0
    .data:0040B7F2                 db    0
    .data:0040B7F3                 db    0
    .data:0040B7F4                 db    0
    .data:0040B7F5                 db    0
    .data:0040B7F6                 db    0
    .data:0040B7F7                 db    0
    .data:0040B7F8                 db    0
    .data:0040B7F9                 db    0
    .data:0040B7FA                 db    0
    .data:0040B7FB                 db    0
    .data:0040B7FC                 db    0
    .data:0040B7FD                 db    0
    .data:0040B7FE                 db    0
    .data:0040B7FF                 db    0
    .data:0040B800                 db    0
    .data:0040B801                 db    0
    .data:0040B802                 db    0
    .data:0040B803                 db    0
    .data:0040B804                 db    0
    .data:0040B805                 db    0
    .data:0040B806                 db    0
    .data:0040B807                 db    0
    .data:0040B808                 db    0
    .data:0040B809                 db    0
    .data:0040B80A                 db    0
    .data:0040B80B                 db    0
    .data:0040B80C                 db    0
    .data:0040B80D                 db    0
    .data:0040B80E                 db    0
    .data:0040B80F                 db    0
    .data:0040B810                 db    0
    .data:0040B811                 db    0
    .data:0040B812                 db    0
    .data:0040B813                 db    0
    .data:0040B814                 db    0
    .data:0040B815                 db    0
    .data:0040B816                 db    0
    .data:0040B817                 db    0
    .data:0040B818                 db    0
    .data:0040B819                 db    0
    .data:0040B81A                 db    0
    .data:0040B81B                 db    0
    .data:0040B81C                 db    0
    .data:0040B81D                 db    0
    .data:0040B81E                 db    0
    .data:0040B81F                 db    0
    .data:0040B820                 db    0
    .data:0040B821                 db    0
    .data:0040B822                 db    0
    .data:0040B823                 db    0
    .data:0040B824                 db    0
    .data:0040B825                 db    0
    .data:0040B826                 db    0
    .data:0040B827                 db    0
    .data:0040B828                 db    0
    .data:0040B829                 db    0
    .data:0040B82A                 db    0
    .data:0040B82B                 db    0
    .data:0040B82C                 db    0
    .data:0040B82D                 db    0
    .data:0040B82E                 db    0
    .data:0040B82F                 db    0
    .data:0040B830                 db    0
    .data:0040B831                 db    0
    .data:0040B832                 db    0
    .data:0040B833                 db    0
    .data:0040B834                 db    0
    .data:0040B835                 db    0
    .data:0040B836                 db    0
    .data:0040B837                 db    0
    .data:0040B838                 db    0
    .data:0040B839                 db    0
    .data:0040B83A                 db    0
    .data:0040B83B                 db    0
    .data:0040B83C                 db    0
    .data:0040B83D                 db    0
    .data:0040B83E                 db    0
    .data:0040B83F                 db    0
    .data:0040B840                 db    0
    .data:0040B841                 db    0
    .data:0040B842                 db    0
    .data:0040B843                 db    0
    .data:0040B844                 db    0
    .data:0040B845                 db    0
    .data:0040B846                 db    0
    .data:0040B847                 db    0
    .data:0040B848                 db    0
    .data:0040B849                 db    0
    .data:0040B84A                 db    0
    .data:0040B84B                 db    0
    .data:0040B84C                 db    0
    .data:0040B84D                 db    0
    .data:0040B84E                 db    0
    .data:0040B84F                 db    0
    .data:0040B850                 db    0
    .data:0040B851                 db    0
    .data:0040B852                 db    0
    .data:0040B853                 db    0
    .data:0040B854                 db    0
    .data:0040B855                 db    0
    .data:0040B856                 db    0
    .data:0040B857                 db    0
    .data:0040B858                 db    0
    .data:0040B859                 db    0
    .data:0040B85A                 db    0
    .data:0040B85B                 db    0
    .data:0040B85C                 db    0
    .data:0040B85D                 db    0
    .data:0040B85E                 db    0
    .data:0040B85F                 db    0
    .data:0040B860                 db    0
    .data:0040B861                 db    0
    .data:0040B862                 db    0
    .data:0040B863                 db    0
    .data:0040B864                 db    0
    .data:0040B865                 db    0
    .data:0040B866                 db    0
    .data:0040B867                 db    0
    .data:0040B868                 db    0
    .data:0040B869                 db    0
    .data:0040B86A                 db    0
    .data:0040B86B                 db    0
    .data:0040B86C                 db    0
    .data:0040B86D                 db    0
    .data:0040B86E                 db    0
    .data:0040B86F                 db    0
    .data:0040B870                 db    0
    .data:0040B871                 db    0
    .data:0040B872                 db    0
    .data:0040B873                 db    0
    .data:0040B874                 db    0
    .data:0040B875                 db    0
    .data:0040B876                 db    0
    .data:0040B877                 db    0
    .data:0040B878                 db    0
    .data:0040B879                 db    0
    .data:0040B87A                 db    0
    .data:0040B87B                 db    0
    .data:0040B87C                 db    0
    .data:0040B87D                 db    0
    .data:0040B87E                 db    0
    .data:0040B87F                 db    0
    .data:0040B880                 db    0
    .data:0040B881                 db    0
    .data:0040B882                 db    0
    .data:0040B883                 db    0
    .data:0040B884                 db    0
    .data:0040B885                 db    0
    .data:0040B886                 db    0
    .data:0040B887                 db    0
    .data:0040B888                 db    0
    .data:0040B889                 db    0
    .data:0040B88A                 db    0
    .data:0040B88B                 db    0
    .data:0040B88C                 db    0
    .data:0040B88D                 db    0
    .data:0040B88E                 db    0
    .data:0040B88F                 db    0
    .data:0040B890                 db    0
    .data:0040B891                 db    0
    .data:0040B892                 db    0
    .data:0040B893                 db    0
    .data:0040B894                 db    0
    .data:0040B895                 db    0
    .data:0040B896                 db    0
    .data:0040B897                 db    0
    .data:0040B898                 db    0
    .data:0040B899                 db    0
    .data:0040B89A                 db    0
    .data:0040B89B                 db    0
    .data:0040B89C                 db    0
    .data:0040B89D                 db    0
    .data:0040B89E                 db    0
    .data:0040B89F                 db    0
    .data:0040B8A0                 db    0
    .data:0040B8A1                 db    0
    .data:0040B8A2                 db    0
    .data:0040B8A3                 db    0
    .data:0040B8A4                 db    0
    .data:0040B8A5                 db    0
    .data:0040B8A6                 db    0
    .data:0040B8A7                 db    0
    .data:0040B8A8                 db    0
    .data:0040B8A9                 db    0
    .data:0040B8AA                 db    0
    .data:0040B8AB                 db    0
    .data:0040B8AC                 db    0
    .data:0040B8AD                 db    0
    .data:0040B8AE                 db    0
    .data:0040B8AF                 db    0
    .data:0040B8B0                 db    0
    .data:0040B8B1                 db    0
    .data:0040B8B2                 db    0
    .data:0040B8B3                 db    0
    .data:0040B8B4                 db    0
    .data:0040B8B5                 db    0
    .data:0040B8B6                 db    0
    .data:0040B8B7                 db    0
    .data:0040B8B8                 db    0
    .data:0040B8B9                 db    0
    .data:0040B8BA                 db    0
    .data:0040B8BB                 db    0
    .data:0040B8BC                 db    0
    .data:0040B8BD                 db    0
    .data:0040B8BE                 db    0
    .data:0040B8BF                 db    0
    .data:0040B8C0                 db    0
    .data:0040B8C1                 db    0
    .data:0040B8C2                 db    0
    .data:0040B8C3                 db    0
    .data:0040B8C4                 db    0
    .data:0040B8C5                 db    0
    .data:0040B8C6                 db    0
    .data:0040B8C7                 db    0
    .data:0040B8C8                 db    0
    .data:0040B8C9                 db    0
    .data:0040B8CA                 db    0
    .data:0040B8CB                 db    0
    .data:0040B8CC                 db    0
    .data:0040B8CD                 db    0
    .data:0040B8CE                 db    0
    .data:0040B8CF                 db    0
    .data:0040B8D0                 db    0
    .data:0040B8D1                 db    0
    .data:0040B8D2                 db    0
    .data:0040B8D3                 db    0
    .data:0040B8D4                 db    0
    .data:0040B8D5                 db    0
    .data:0040B8D6                 db    0
    .data:0040B8D7                 db    0
    .data:0040B8D8                 db    0
    .data:0040B8D9                 db    0
    .data:0040B8DA                 db    0
    .data:0040B8DB                 db    0
    .data:0040B8DC                 db    0
    .data:0040B8DD                 db    0
    .data:0040B8DE                 db    0
    .data:0040B8DF                 db    0
    .data:0040B8E0                 db    0
    .data:0040B8E1                 db    0
    .data:0040B8E2                 db    0
    .data:0040B8E3                 db    0
    .data:0040B8E4                 db    0
    .data:0040B8E5                 db    0
    .data:0040B8E6                 db    0
    .data:0040B8E7                 db    0
    .data:0040B8E8                 db    0
    .data:0040B8E9                 db    0
    .data:0040B8EA                 db    0
    .data:0040B8EB                 db    0
    .data:0040B8EC                 db    0
    .data:0040B8ED                 db    0
    .data:0040B8EE                 db    0
    .data:0040B8EF                 db    0
    .data:0040B8F0                 db    0
    .data:0040B8F1                 db    0
    .data:0040B8F2                 db    0
    .data:0040B8F3                 db    0
    .data:0040B8F4                 db    0
    .data:0040B8F5                 db    0
    .data:0040B8F6                 db    0
    .data:0040B8F7                 db    0
    .data:0040B8F8                 db    0
    .data:0040B8F9                 db    0
    .data:0040B8FA                 db    0
    .data:0040B8FB                 db    0
    .data:0040B8FC                 db    0
    .data:0040B8FD                 db    0
    .data:0040B8FE                 db    0
    .data:0040B8FF                 db    0
    .data:0040B900                 db    0
    .data:0040B901                 db    0
    .data:0040B902                 db    0
    .data:0040B903                 db    0
    .data:0040B904                 db    0
    .data:0040B905                 db    0
    .data:0040B906                 db    0
    .data:0040B907                 db    0
    .data:0040B908                 db    0
    .data:0040B909                 db    0
    .data:0040B90A                 db    0
    .data:0040B90B                 db    0
    .data:0040B90C                 db    0
    .data:0040B90D                 db    0
    .data:0040B90E                 db    0
    .data:0040B90F                 db    0
    .data:0040B910                 db    0
    .data:0040B911                 db    0
    .data:0040B912                 db    0
    .data:0040B913                 db    0
    .data:0040B914                 db    0
    .data:0040B915                 db    0
    .data:0040B916                 db    0
    .data:0040B917                 db    0
    .data:0040B918                 db    0
    .data:0040B919                 db    0
    .data:0040B91A                 db    0
    .data:0040B91B                 db    0
    .data:0040B91C                 db    0
    .data:0040B91D                 db    0
    .data:0040B91E                 db    0
    .data:0040B91F                 db    0
    .data:0040B920                 db    0
    .data:0040B921                 db    0
    .data:0040B922                 db    0
    .data:0040B923                 db    0
    .data:0040B924                 db    0
    .data:0040B925                 db    0
    .data:0040B926                 db    0
    .data:0040B927                 db    0
    .data:0040B928                 db    0
    .data:0040B929                 db    0
    .data:0040B92A                 db    0
    .data:0040B92B                 db    0
    .data:0040B92C                 db    0
    .data:0040B92D                 db    0
    .data:0040B92E                 db    0
    .data:0040B92F                 db    0
    .data:0040B930                 db    0
    .data:0040B931                 db    0
    .data:0040B932                 db    0
    .data:0040B933                 db    0
    .data:0040B934                 db    0
    .data:0040B935                 db    0
    .data:0040B936                 db    0
    .data:0040B937                 db    0
    .data:0040B938                 db    0
    .data:0040B939                 db    0
    .data:0040B93A                 db    0
    .data:0040B93B                 db    0
    .data:0040B93C                 db    0
    .data:0040B93D                 db    0
    .data:0040B93E                 db    0
    .data:0040B93F                 db    0
    .data:0040B940                 db    0
    .data:0040B941                 db    0
    .data:0040B942                 db    0
    .data:0040B943                 db    0
    .data:0040B944                 db    0
    .data:0040B945                 db    0
    .data:0040B946                 db    0
    .data:0040B947                 db    0
    .data:0040B948                 db    0
    .data:0040B949                 db    0
    .data:0040B94A                 db    0
    .data:0040B94B                 db    0
    .data:0040B94C                 db    0
    .data:0040B94D                 db    0
    .data:0040B94E                 db    0
    .data:0040B94F                 db    0
    .data:0040B950                 db    0
    .data:0040B951                 db    0
    .data:0040B952                 db    0
    .data:0040B953                 db    0
    .data:0040B954                 db    0
    .data:0040B955                 db    0
    .data:0040B956                 db    0
    .data:0040B957                 db    0
    .data:0040B958                 db    0
    .data:0040B959                 db    0
    .data:0040B95A                 db    0
    .data:0040B95B                 db    0
    .data:0040B95C                 db    0
    .data:0040B95D                 db    0
    .data:0040B95E                 db    0
    .data:0040B95F                 db    0
    .data:0040B960                 db    0
    .data:0040B961                 db    0
    .data:0040B962                 db    0
    .data:0040B963                 db    0
    .data:0040B964                 db    0
    .data:0040B965                 db    0
    .data:0040B966                 db    0
    .data:0040B967                 db    0
    .data:0040B968                 db    0
    .data:0040B969                 db    0
    .data:0040B96A                 db    0
    .data:0040B96B                 db    0
    .data:0040B96C                 db    0
    .data:0040B96D                 db    0
    .data:0040B96E                 db    0
    .data:0040B96F                 db    0
    .data:0040B970                 db    0
    .data:0040B971                 db    0
    .data:0040B972                 db    0
    .data:0040B973                 db    0
    .data:0040B974                 db    0
    .data:0040B975                 db    0
    .data:0040B976                 db    0
    .data:0040B977                 db    0
    .data:0040B978                 db    0
    .data:0040B979                 db    0
    .data:0040B97A                 db    0
    .data:0040B97B                 db    0
    .data:0040B97C                 db    0
    .data:0040B97D                 db    0
    .data:0040B97E                 db    0
    .data:0040B97F                 db    0
    .data:0040B980                 db    0
    .data:0040B981                 db    0
    .data:0040B982                 db    0
    .data:0040B983                 db    0
    .data:0040B984                 db    0
    .data:0040B985                 db    0
    .data:0040B986                 db    0
    .data:0040B987                 db    0
    .data:0040B988                 db    0
    .data:0040B989                 db    0
    .data:0040B98A                 db    0
    .data:0040B98B                 db    0
    .data:0040B98C                 db    0
    .data:0040B98D                 db    0
    .data:0040B98E                 db    0
    .data:0040B98F                 db    0
    .data:0040B990                 db    0
    .data:0040B991                 db    0
    .data:0040B992                 db    0
    .data:0040B993                 db    0
    .data:0040B994                 db    0
    .data:0040B995                 db    0
    .data:0040B996                 db    0
    .data:0040B997                 db    0
    .data:0040B998                 db    0
    .data:0040B999                 db    0
    .data:0040B99A                 db    0
    .data:0040B99B                 db    0
    .data:0040B99C                 db    0
    .data:0040B99D                 db    0
    .data:0040B99E                 db    0
    .data:0040B99F                 db    0
    .data:0040B9A0                 db    0
    .data:0040B9A1                 db    0
    .data:0040B9A2                 db    0
    .data:0040B9A3                 db    0
    .data:0040B9A4                 db    0
    .data:0040B9A5                 db    0
    .data:0040B9A6                 db    0
    .data:0040B9A7                 db    0
    .data:0040B9A8                 db    0
    .data:0040B9A9                 db    0
    .data:0040B9AA                 db    0
    .data:0040B9AB                 db    0
    .data:0040B9AC                 db    0
    .data:0040B9AD                 db    0
    .data:0040B9AE                 db    0
    .data:0040B9AF                 db    0
    .data:0040B9B0                 db    0
    .data:0040B9B1                 db    0
    .data:0040B9B2                 db    0
    .data:0040B9B3                 db    0
    .data:0040B9B4                 db    0
    .data:0040B9B5                 db    0
    .data:0040B9B6                 db    0
    .data:0040B9B7                 db    0
    .data:0040B9B8                 db    0
    .data:0040B9B9                 db    0
    .data:0040B9BA                 db    0
    .data:0040B9BB                 db    0
    .data:0040B9BC                 db    0
    .data:0040B9BD                 db    0
    .data:0040B9BE                 db    0
    .data:0040B9BF                 db    0
    
    .data:0040A408 unk_40A408      db  9Eh ; P             ; DATA XREF: _main+50o
    .data:0040A409                 db 0A2h ; ó
    .data:0040A40A                 db  6Bh ; k
    .data:0040A40B                 db  46h ; F
    .data:0040A40C                 db  99h ; Ö
    .data:0040A40D                 db  35h ; 5
    .data:0040A40E                 db  8Bh ; ï
    .data:0040A40F                 db  7Ch ; |
    .data:0040A410                 db 0BAh ; ¦
    .data:0040A411                 db 0C5h ; +
    .data:0040A412                 db 0ADh ; ¡
    .data:0040A413                 db  19h
    .data:0040A414                 db  7Bh ; {
    .data:0040A415                 db  79h ; y
    .data:0040A416                 db 0FBh ; v
    .data:0040A417                 db 0F9h ; ·
    .data:0040A418                 db  4Ah ; J
    .data:0040A419                 db  2Eh ; .
    .data:0040A41A                 db  3Ah ; :
    .data:0040A41B                 db  0Ch
    .data:0040A41C                 db  0Ch
    .data:0040A41D                 db  5Fh ; _
    .data:0040A41E                 db  9Bh ; ¢
    .data:0040A41F                 db 0A7h ; º
    .data:0040A420                 db  43h ; C
    .data:0040A421                 db 0CCh ; ¦
    .data:0040A422                 db 0C0h ; +
    .data:0040A423                 db 0D7h ; +
    .data:0040A424                 db  6Eh ; n
    .data:0040A425                 db 0E2h ; G
    .data:0040A426                 db 0DEh ; ¦
    .data:0040A427                 db 0C0h ; +
    .data:0040A428                 db  4Dh ; M
    .data:0040A429                 db 0D5h ; +
    .data:0040A42A                 db 0DDh ; ¦
    .data:0040A42B                 db 0C6h ; ¦
    .data:0040A42C                 db  71h ; q
    .data:0040A42D                 db 0DCh ; _
    .data:0040A42E                 db 0D0h ; -
    .data:0040A42F                 db 0C0h ; +
    .data:0040A430                 db  4Dh ; M
    .data:0040A431                 db 0D5h ; +
    .data:0040A432                 db 0DEh ; ¦
    .data:0040A433                 db 0CFh ; -
    .data:0040A434                 db  7Dh ; }
    .data:0040A435                 db 0DFh ; ¯
    .data:0040A436                 db 0DBh ; ¦
    .data:0040A437                 db 0C0h ; +
    .data:0040A438                 db  7Bh ; {
    .data:0040A439                 db 0D5h ; +
    .data:0040A43A                 db 0CEh ; +
    .data:0040A43B                 db 0C9h ; +
    .data:0040A43C                 db  72h ; r
    .data:0040A43D                 db 0E0h ; a
    .data:0040A43E                 db 0DFh ; ¯
    .data:0040A43F                 db 0C3h ; +
    .data:0040A440                 db  57h ; W
    .data:0040A441                 db 0D9h ; +
    .data:0040A442                 db 0D6h ; +
    .data:0040A443                 db 0D3h ; +
    .data:0040A444                 db  75h ; u
    .data:0040A445                 db 0D1h ; -
    .data:0040A446                 db 0E0h ; a
    .data:0040A447                 db 0D7h ; +
    .data:0040A448                 db  3Bh ; ;
    .data:0040A449                 db 0A1h ; í
    .data:0040A44A                 db 0A3h ; ú
    .data:0040A44B                 db  92h ; Æ
    .data:0040A44C                 db  7Bh ; {
    .data:0040A44D                 db 0E4h ; S
    .data:0040A44E                 db 0D1h ; -
    .data:0040A44F                 db  64h ; d
    .data:0040A450                 db  4Eh ; N
    .data:0040A451                 db  1Fh
    .data:0040A452                 db  5Ch ; \
    .data:0040A453                 db    2
    .data:0040A454                 db 0F0h ; =
    .data:0040A455                 db 0CEh ; +
    .data:0040A456                 db  0Fh
    .data:0040A457                 db  6Ah ; j
    .data:0040A458                 db  4Eh ; N
    .data:0040A459                 db  1Dh
    .data:0040A45A                 db 0ECh ; 8
    .data:0040A45B                 db  9Ch ; £
    .data:0040A45C                 db 0F4h ; (
    .data:0040A45D                 db  9Bh ; ¢
    .data:0040A45E                 db  30h ; 0
    .data:0040A45F                 db  44h ; D
    .data:0040A460                 db  0Eh
    .data:0040A461                 db 0F4h ; (
    .data:0040A462                 db  35h ; 5
    .data:0040A463                 db  8Dh ; ì
    .data:0040A464                 db  92h ; Æ
    .data:0040A465                 db  92h ; Æ
    .data:0040A466                 db  7Dh ; }
    .data:0040A467                 db  6Fh ; o
    .data:0040A468                 db  6Ah ; j
    .data:0040A469                 db  14h
    .data:0040A46A                 db 0E9h ; T
    .data:0040A46B                 db 0C9h ; +
    .data:0040A46C                 db  29h ; )
    .data:0040A46D                 db 0E1h ; ß
    .data:0040A46E                 db  8Ah ; è
    .data:0040A46F                 db  4Eh ; N
    .data:0040A470                 db 0DFh ; ¯
    .data:0040A471                 db  91h ; æ
    .data:0040A472                 db    9
    .data:0040A473                 db    1
    .data:0040A474                 db 0B3h ; ¦
    .data:0040A475                 db 0EEh ; e
    .data:0040A476                 db  98h ; ÿ
    .data:0040A477                 db  49h ; I
    .data:0040A478                 db 0ACh ; ¼
    .data:0040A479                 db  5Ah ; Z
    .data:0040A47A                 db  67h ; g
    .data:0040A47B                 db 0E6h ; µ
    .data:0040A47C                 db  75h ; u
    .data:0040A47D                 db  5Fh ; _
    .data:0040A47E                 db  74h ; t
    .data:0040A47F                 db  3Eh ; >
    .data:0040A480                 db  7Bh ; {
    .data:0040A481                 db  9Fh ; ƒ
    .data:0040A482                 db 0D7h ; +
    .data:0040A483                 db 0CBh ; -
    .data:0040A484                 db  28h ; (
    .data:0040A485                 db  7Bh ; {
    .data:0040A486                 db  5Ah ; Z
    .data:0040A487                 db 0C0h ; +
    .data:0040A488                 db  23h ; #
    .data:0040A489                 db  9Fh ; ƒ
    .data:0040A48A                 db  5Ch ; \
    .data:0040A48B                 db    5
    .data:0040A48C                 db  4Ch ; L
    .data:0040A48D                 db  53h ; S
    .data:0040A48E                 db  77h ; w
    .data:0040A48F                 db  2Eh ; .
    .data:0040A490                 db  75h ; u
    .data:0040A491                 db 0B6h ; ¦
    .data:0040A492                 db 0E3h ; p
    .data:0040A493                 db  25h ; %
    .data:0040A494                 db  75h ; u
    .data:0040A495                 db 0C1h ; -
    .data:0040A496                 db  6Eh ; n
    .data:0040A497                 db  87h ; ç
    .data:0040A498                 db  9Dh ; ¥
    .data:0040A499                 db 0C5h ; +
    .data:0040A49A                 db 0A3h ; ú
    .data:0040A49B                 db    3
    .data:0040A49C                 db 0B8h ; +
    .data:0040A49D                 db 0B4h ; ¦
    .data:0040A49E                 db 0F5h ; )
    .data:0040A49F                 db 0A9h ; ¬
    .data:0040A4A0                 db  8Eh ; Ä
    .data:0040A4A1                 db  68h ; h
    .data:0040A4A2                 db  78h ; x
    .data:0040A4A3                 db  95h ; ò
    .data:0040A4A4                 db  9Dh ; ¥
    .data:0040A4A5                 db 0C9h ; +
    .data:0040A4A6                 db    2
    .data:0040A4A7                 db  47h ; G
    .data:0040A4A8                 db  80h ; Ç
    .data:0040A4A9                 db 0F3h ; =
    .data:0040A4AA                 db 0D2h ; -
    .data:0040A4AB                 db  1Bh
    .data:0040A4AC                 db 0ABh ; ½
    .data:0040A4AD                 db 0BEh ; +
    .data:0040A4AE                 db 0FCh ; n
    .data:0040A4AF                 db  3Eh ; >
    .data:0040A4B0                 db  82h ; é
    .data:0040A4B1                 db  51h ; Q
    .data:0040A4B2                 db  42h ; B
    .data:0040A4B3                 db  8Dh ; ì
    .data:0040A4B4                 db  76h ; v
    .data:0040A4B5                 db 0A8h ; ¿
    .data:0040A4B6                 db  95h ; ò
    .data:0040A4B7                 db  34h ; 4
    .data:0040A4B8                 db  95h ; ò
    .data:0040A4B9                 db 0A0h ; á
    .data:0040A4BA                 db    1
    .data:0040A4BB                 db  74h ; t
    .data:0040A4BC                 db 0CFh ; -
    .data:0040A4BD                 db    5
    .data:0040A4BE                 db  94h ; ö
    .data:0040A4BF                 db  0Bh
    .data:0040A4C0                 db  5Ch ; \
    .data:0040A4C1                 db  2Bh ; +
    .data:0040A4C2                 db  1Bh
    .data:0040A4C3                 db  73h ; s
    .data:0040A4C4                 db  74h ; t
    .data:0040A4C5                 db  15h
    .data:0040A4C6                 db 0CBh ; -
    .data:0040A4C7                 db  1Bh
    .data:0040A4C8                 db 0D9h ; +
    .data:0040A4C9                 db 0AAh ; ¬
    .data:0040A4CA                 db  1Fh
    .data:0040A4CB                 db  38h ; 8
    .data:0040A4CC                 db  59h ; Y
    .data:0040A4CD                 db  85h ; à
    .data:0040A4CE                 db  0Eh
    .data:0040A4CF                 db  4Dh ; M
    .data:0040A4D0                 db 0C0h ; +
    .data:0040A4D1                 db 0D9h ; +
    .data:0040A4D2                 db 0DDh ; ¦
    .data:0040A4D3                 db  30h ; 0
    .data:0040A4D4                 db  7Ch ; |
    .data:0040A4D5                 db 0F2h ; =
    .data:0040A4D6                 db 0B8h ; +
    .data:0040A4D7                 db  72h ; r
    .data:0040A4D8                 db  4Fh ; O
    .data:0040A4D9                 db 0DEh ; ¦
    .data:0040A4DA                 db  41h ; A
    .data:0040A4DB                 db  16h
    .data:0040A4DC                 db 0D1h ; -
    .data:0040A4DD                 db  31h ; 1
    .data:0040A4DE                 db 0D3h ; +
    .data:0040A4DF                 db  78h ; x
    .data:0040A4E0                 db  40h ; @
    .data:0040A4E1                 db  7Bh ; {
    .data:0040A4E2                 db 0AEh ; «
    .data:0040A4E3                 db 0C3h ; +
    .data:0040A4E4                 db  34h ; 4
    .data:0040A4E5                 db 0E8h ; F
    .data:0040A4E6                 db 0B4h ; ¦
    .data:0040A4E7                 db  68h ; h
    .data:0040A4E8                 db  4Ah ; J
    .data:0040A4E9                 db  12h
    .data:0040A4EA                 db  74h ; t
    .data:0040A4EB                 db  5Fh ; _
    .data:0040A4EC                 db 0EDh ; f
    .data:0040A4ED                 db  83h ; â
    .data:0040A4EE                 db 0BCh ; +
    .data:0040A4EF                 db 0BBh ; +
    .data:0040A4F0                 db  2Ah ; *
    .data:0040A4F1                 db 0FAh ; ·
    .data:0040A4F2                 db 0D3h ; +
    .data:0040A4F3                 db 0D2h ; -
    .data:0040A4F4                 db  50h ; P
    .data:0040A4F5                 db  68h ; h
    .data:0040A4F6                 db 0A6h ; ª
    .data:0040A4F7                 db  77h ; w
    .data:0040A4F8                 db  46h ; F
    .data:0040A4F9                 db  29h ; )
    .data:0040A4FA                 db  8Ah ; è
    .data:0040A4FB                 db  92h ; Æ
    .data:0040A4FC                 db  58h ; X
    .data:0040A4FD                 db  8Bh ; ï
    .data:0040A4FE                 db  59h ; Y
    .data:0040A4FF                 db  9Dh ; ¥
    .data:0040A500                 db 0D8h ; +
    .data:0040A501                 db  1Eh
    .data:0040A502                 db  7Fh ; 
    .data:0040A503                 db 0B7h ; +
    .data:0040A504                 db  66h ; f
    .data:0040A505                 db  45h ; E
    .data:0040A506                 db 0DAh ; +
    .data:0040A507                 db    0
    
    .data:0040BBC0 ; const WCHAR FileName
    .data:0040BBC0 FileName        dw 0                    ; DATA XREF: _main+4Bo
    .data:0040BBC0                                         ; _main+8Eo
    .data:0040BBC2                 db    0
    .data:0040BBC3                 db    0
    .data:0040BBC4                 db    0
    .data:0040BBC5                 db    0
    .data:0040BBC6                 db    0
    .data:0040BBC7                 db    0
    .data:0040BBC8                 db    0
    .data:0040BBC9                 db    0
    .data:0040BBCA                 db    0
    .data:0040BBCB                 db    0
    .data:0040BBCC                 db    0
    .data:0040BBCD                 db    0
    .data:0040BBCE                 db    0
    .data:0040BBCF                 db    0
    .data:0040BBD0                 db    0
    .data:0040BBD1                 db    0
    .data:0040BBD2                 db    0
    .data:0040BBD3                 db    0
    .data:0040BBD4                 db    0
    .data:0040BBD5                 db    0
    .data:0040BBD6                 db    0
    .data:0040BBD7                 db    0
    .data:0040BBD8                 db    0
    .data:0040BBD9                 db    0
    .data:0040BBDA                 db    0
    .data:0040BBDB                 db    0
    .data:0040BBDC                 db    0
    .data:0040BBDD                 db    0
    .data:0040BBDE                 db    0
    .data:0040BBDF                 db    0
    .data:0040BBE0                 db    0
    .data:0040BBE1                 db    0
    .data:0040BBE2                 db    0
    .data:0040BBE3                 db    0
    .data:0040BBE4                 db    0
    .data:0040BBE5                 db    0
    .data:0040BBE6                 db    0
    .data:0040BBE7                 db    0
    .data:0040BBE8                 db    0
    .data:0040BBE9                 db    0
    .data:0040BBEA                 db    0
    .data:0040BBEB                 db    0
    .data:0040BBEC                 db    0
    .data:0040BBED                 db    0
    .data:0040BBEE                 db    0
    .data:0040BBEF                 db    0
    .data:0040BBF0                 db    0
    .data:0040BBF1                 db    0
    .data:0040BBF2                 db    0
    .data:0040BBF3                 db    0
    .data:0040BBF4                 db    0
    .data:0040BBF5                 db    0
    .data:0040BBF6                 db    0
    .data:0040BBF7                 db    0
    .data:0040BBF8                 db    0
    .data:0040BBF9                 db    0
    .data:0040BBFA                 db    0
    .data:0040BBFB                 db    0
    .data:0040BBFC                 db    0
    .data:0040BBFD                 db    0
    .data:0040BBFE                 db    0
    .data:0040BBFF                 db    0
    .data:0040BC00                 db    0
    .data:0040BC01                 db    0
    .data:0040BC02                 db    0
    .data:0040BC03                 db    0
    .data:0040BC04                 db    0
    .data:0040BC05                 db    0
    .data:0040BC06                 db    0
    .data:0040BC07                 db    0
    .data:0040BC08                 db    0
    .data:0040BC09                 db    0
    .data:0040BC0A                 db    0
    .data:0040BC0B                 db    0
    .data:0040BC0C                 db    0
    .data:0040BC0D                 db    0
    .data:0040BC0E                 db    0
    .data:0040BC0F                 db    0
    .data:0040BC10                 db    0
    .data:0040BC11                 db    0
    .data:0040BC12                 db    0
    .data:0040BC13                 db    0
    .data:0040BC14                 db    0
    .data:0040BC15                 db    0
    .data:0040BC16                 db    0
    .data:0040BC17                 db    0
    .data:0040BC18                 db    0
    .data:0040BC19                 db    0
    .data:0040BC1A                 db    0
    .data:0040BC1B                 db    0
    .data:0040BC1C                 db    0
    .data:0040BC1D                 db    0
    .data:0040BC1E                 db    0
    .data:0040BC1F                 db    0
    .data:0040BC20                 db    0
    .data:0040BC21                 db    0
    .data:0040BC22                 db    0
    .data:0040BC23                 db    0
    .data:0040BC24                 db    0
    .data:0040BC25                 db    0
    .data:0040BC26                 db    0
    .data:0040BC27                 db    0
    .data:0040BC28                 db    0
    .data:0040BC29                 db    0
    .data:0040BC2A                 db    0
    .data:0040BC2B                 db    0
    .data:0040BC2C                 db    0
    .data:0040BC2D                 db    0
    .data:0040BC2E                 db    0
    .data:0040BC2F                 db    0
    .data:0040BC30                 db    0
    .data:0040BC31                 db    0
    .data:0040BC32                 db    0
    .data:0040BC33                 db    0
    .data:0040BC34                 db    0
    .data:0040BC35                 db    0
    .data:0040BC36                 db    0
    .data:0040BC37                 db    0
    .data:0040BC38                 db    0
    .data:0040BC39                 db    0
    .data:0040BC3A                 db    0
    .data:0040BC3B                 db    0
    .data:0040BC3C                 db    0
    .data:0040BC3D                 db    0
    .data:0040BC3E                 db    0
    .data:0040BC3F                 db    0
    .data:0040BC40                 db    0
    .data:0040BC41                 db    0
    .data:0040BC42                 db    0
    .data:0040BC43                 db    0
    .data:0040BC44                 db    0
    .data:0040BC45                 db    0
    .data:0040BC46                 db    0
    .data:0040BC47                 db    0
    .data:0040BC48                 db    0
    .data:0040BC49                 db    0
    .data:0040BC4A                 db    0
    .data:0040BC4B                 db    0
    .data:0040BC4C                 db    0
    .data:0040BC4D                 db    0
    .data:0040BC4E                 db    0
    .data:0040BC4F                 db    0
    .data:0040BC50                 db    0
    .data:0040BC51                 db    0
    .data:0040BC52                 db    0
    .data:0040BC53                 db    0
    .data:0040BC54                 db    0
    .data:0040BC55                 db    0
    .data:0040BC56                 db    0
    .data:0040BC57                 db    0
    .data:0040BC58                 db    0
    .data:0040BC59                 db    0
    .data:0040BC5A                 db    0
    .data:0040BC5B                 db    0
    .data:0040BC5C                 db    0
    .data:0040BC5D                 db    0
    .data:0040BC5E                 db    0
    .data:0040BC5F                 db    0
    .data:0040BC60                 db    0
    .data:0040BC61                 db    0
    .data:0040BC62                 db    0
    .data:0040BC63                 db    0
    .data:0040BC64                 db    0
    .data:0040BC65                 db    0
    .data:0040BC66                 db    0
    .data:0040BC67                 db    0
    .data:0040BC68                 db    0
    .data:0040BC69                 db    0
    .data:0040BC6A                 db    0
    .data:0040BC6B                 db    0
    .data:0040BC6C                 db    0
    .data:0040BC6D                 db    0
    .data:0040BC6E                 db    0
    .data:0040BC6F                 db    0
    .data:0040BC70                 db    0
    .data:0040BC71                 db    0
    .data:0040BC72                 db    0
    .data:0040BC73                 db    0
    .data:0040BC74                 db    0
    .data:0040BC75                 db    0
    .data:0040BC76                 db    0
    .data:0040BC77                 db    0
    .data:0040BC78                 db    0
    .data:0040BC79                 db    0
    .data:0040BC7A                 db    0
    .data:0040BC7B                 db    0
    .data:0040BC7C                 db    0
    .data:0040BC7D                 db    0
    .data:0040BC7E                 db    0
    .data:0040BC7F                 db    0
    .data:0040BC80                 db    0
    .data:0040BC81                 db    0
    .data:0040BC82                 db    0
    .data:0040BC83                 db    0
    .data:0040BC84                 db    0
    .data:0040BC85                 db    0
    .data:0040BC86                 db    0
    .data:0040BC87                 db    0
    .data:0040BC88                 db    0
    .data:0040BC89                 db    0
    .data:0040BC8A                 db    0
    .data:0040BC8B                 db    0
    .data:0040BC8C                 db    0
    .data:0040BC8D                 db    0
    .data:0040BC8E                 db    0
    .data:0040BC8F                 db    0
    .data:0040BC90                 db    0
    .data:0040BC91                 db    0
    .data:0040BC92                 db    0
    .data:0040BC93                 db    0
    .data:0040BC94                 db    0
    .data:0040BC95                 db    0
    .data:0040BC96                 db    0
    .data:0040BC97                 db    0
    .data:0040BC98                 db    0
    .data:0040BC99                 db    0
    .data:0040BC9A                 db    0
    .data:0040BC9B                 db    0
    .data:0040BC9C                 db    0
    .data:0040BC9D                 db    0
    .data:0040BC9E                 db    0
    .data:0040BC9F                 db    0
    .data:0040BCA0                 db    0
    .data:0040BCA1                 db    0
    .data:0040BCA2                 db    0
    .data:0040BCA3                 db    0
    .data:0040BCA4                 db    0
    .data:0040BCA5                 db    0
    .data:0040BCA6                 db    0
    .data:0040BCA7                 db    0
    .data:0040BCA8                 db    0
    .data:0040BCA9                 db    0
    .data:0040BCAA                 db    0
    .data:0040BCAB                 db    0
    .data:0040BCAC                 db    0
    .data:0040BCAD                 db    0
    .data:0040BCAE                 db    0
    .data:0040BCAF                 db    0
    .data:0040BCB0                 db    0
    .data:0040BCB1                 db    0
    .data:0040BCB2                 db    0
    .data:0040BCB3                 db    0
    .data:0040BCB4                 db    0
    .data:0040BCB5                 db    0
    .data:0040BCB6                 db    0
    .data:0040BCB7                 db    0
    .data:0040BCB8                 db    0
    .data:0040BCB9                 db    0
    .data:0040BCBA                 db    0
    .data:0040BCBB                 db    0
    .data:0040BCBC                 db    0
    .data:0040BCBD                 db    0
    .data:0040BCBE                 db    0
    .data:0040BCBF                 db    0
    .data:0040BCC0                 db    0
    .data:0040BCC1                 db    0
    .data:0040BCC2                 db    0
    .data:0040BCC3                 db    0
    .data:0040BCC4                 db    0
    .data:0040BCC5                 db    0
    .data:0040BCC6                 db    0
    .data:0040BCC7                 db    0
    .data:0040BCC8                 db    0
    .data:0040BCC9                 db    0
    .data:0040BCCA                 db    0
    .data:0040BCCB                 db    0
    .data:0040BCCC                 db    0
    .data:0040BCCD                 db    0
    .data:0040BCCE                 db    0
    .data:0040BCCF                 db    0
    .data:0040BCD0                 db    0
    .data:0040BCD1                 db    0
    .data:0040BCD2                 db    0
    .data:0040BCD3                 db    0
    .data:0040BCD4                 db    0
    .data:0040BCD5                 db    0
    .data:0040BCD6                 db    0
    .data:0040BCD7                 db    0
    .data:0040BCD8                 db    0
    .data:0040BCD9                 db    0
    .data:0040BCDA                 db    0
    .data:0040BCDB                 db    0
    .data:0040BCDC                 db    0
    .data:0040BCDD                 db    0
    .data:0040BCDE                 db    0
    .data:0040BCDF                 db    0
    .data:0040BCE0                 db    0
    .data:0040BCE1                 db    0
    .data:0040BCE2                 db    0
    .data:0040BCE3                 db    0
    .data:0040BCE4                 db    0
    .data:0040BCE5                 db    0
    .data:0040BCE6                 db    0
    .data:0040BCE7                 db    0
    .data:0040BCE8                 db    0
    .data:0040BCE9                 db    0
    .data:0040BCEA                 db    0
    .data:0040BCEB                 db    0
    .data:0040BCEC                 db    0
    .data:0040BCED                 db    0
    .data:0040BCEE                 db    0
    .data:0040BCEF                 db    0
    .data:0040BCF0                 db    0
    .data:0040BCF1                 db    0
    .data:0040BCF2                 db    0
    .data:0040BCF3                 db    0
    .data:0040BCF4                 db    0
    .data:0040BCF5                 db    0
    .data:0040BCF6                 db    0
    .data:0040BCF7                 db    0
    .data:0040BCF8                 db    0
    .data:0040BCF9                 db    0
    .data:0040BCFA                 db    0
    .data:0040BCFB                 db    0
    .data:0040BCFC                 db    0
    .data:0040BCFD                 db    0
    .data:0040BCFE                 db    0
    .data:0040BCFF                 db    0
    .data:0040BD00                 db    0
    .data:0040BD01                 db    0
    .data:0040BD02                 db    0
    .data:0040BD03                 db    0
    .data:0040BD04                 db    0
    .data:0040BD05                 db    0
    .data:0040BD06                 db    0
    .data:0040BD07                 db    0
    .data:0040BD08                 db    0
    .data:0040BD09                 db    0
    .data:0040BD0A                 db    0
    .data:0040BD0B                 db    0
    .data:0040BD0C                 db    0
    .data:0040BD0D                 db    0
    .data:0040BD0E                 db    0
    .data:0040BD0F                 db    0
    .data:0040BD10                 db    0
    .data:0040BD11                 db    0
    .data:0040BD12                 db    0
    .data:0040BD13                 db    0
    .data:0040BD14                 db    0
    .data:0040BD15                 db    0
    .data:0040BD16                 db    0
    .data:0040BD17                 db    0
    .data:0040BD18                 db    0
    .data:0040BD19                 db    0
    .data:0040BD1A                 db    0
    .data:0040BD1B                 db    0
    .data:0040BD1C                 db    0
    .data:0040BD1D                 db    0
    .data:0040BD1E                 db    0
    .data:0040BD1F                 db    0
    .data:0040BD20                 db    0
    .data:0040BD21                 db    0
    .data:0040BD22                 db    0
    .data:0040BD23                 db    0
    .data:0040BD24                 db    0
    .data:0040BD25                 db    0
    .data:0040BD26                 db    0
    .data:0040BD27                 db    0
    .data:0040BD28                 db    0
    .data:0040BD29                 db    0
    .data:0040BD2A                 db    0
    .data:0040BD2B                 db    0
    .data:0040BD2C                 db    0
    .data:0040BD2D                 db    0
    .data:0040BD2E                 db    0
    .data:0040BD2F                 db    0
    .data:0040BD30                 db    0
    .data:0040BD31                 db    0
    .data:0040BD32                 db    0
    .data:0040BD33                 db    0
    .data:0040BD34                 db    0
    .data:0040BD35                 db    0
    .data:0040BD36                 db    0
    .data:0040BD37                 db    0
    .data:0040BD38                 db    0
    .data:0040BD39                 db    0
    .data:0040BD3A                 db    0
    .data:0040BD3B                 db    0
    .data:0040BD3C                 db    0
    .data:0040BD3D                 db    0
    .data:0040BD3E                 db    0
    .data:0040BD3F                 db    0
    .data:0040BD40                 db    0
    .data:0040BD41                 db    0
    .data:0040BD42                 db    0
    .data:0040BD43                 db    0
    .data:0040BD44                 db    0
    .data:0040BD45                 db    0
    .data:0040BD46                 db    0
    .data:0040BD47                 db    0
    .data:0040BD48                 db    0
    .data:0040BD49                 db    0
    .data:0040BD4A                 db    0
    .data:0040BD4B                 db    0
    .data:0040BD4C                 db    0
    .data:0040BD4D                 db    0
    .data:0040BD4E                 db    0
    .data:0040BD4F                 db    0
    .data:0040BD50                 db    0
    .data:0040BD51                 db    0
    .data:0040BD52                 db    0
    .data:0040BD53                 db    0
    .data:0040BD54                 db    0
    .data:0040BD55                 db    0
    .data:0040BD56                 db    0
    .data:0040BD57                 db    0
    .data:0040BD58                 db    0
    .data:0040BD59                 db    0
    .data:0040BD5A                 db    0
    .data:0040BD5B                 db    0
    .data:0040BD5C                 db    0
    .data:0040BD5D                 db    0
    .data:0040BD5E                 db    0
    .data:0040BD5F                 db    0
    .data:0040BD60                 db    0
    .data:0040BD61                 db    0
    .data:0040BD62                 db    0
    .data:0040BD63                 db    0
    .data:0040BD64                 db    0
    .data:0040BD65                 db    0
    .data:0040BD66                 db    0
    .data:0040BD67                 db    0
    .data:0040BD68                 db    0
    .data:0040BD69                 db    0
    .data:0040BD6A                 db    0
    .data:0040BD6B                 db    0
    .data:0040BD6C                 db    0
    .data:0040BD6D                 db    0
    .data:0040BD6E                 db    0
    .data:0040BD6F                 db    0
    .data:0040BD70                 db    0
    .data:0040BD71                 db    0
    .data:0040BD72                 db    0
    .data:0040BD73                 db    0
    .data:0040BD74                 db    0
    .data:0040BD75                 db    0
    .data:0040BD76                 db    0
    .data:0040BD77                 db    0
    .data:0040BD78                 db    0
    .data:0040BD79                 db    0
    .data:0040BD7A                 db    0
    .data:0040BD7B                 db    0
    .data:0040BD7C                 db    0
    .data:0040BD7D                 db    0
    .data:0040BD7E                 db    0
    .data:0040BD7F                 db    0
    .data:0040BD80                 db    0
    .data:0040BD81                 db    0
    .data:0040BD82                 db    0
    .data:0040BD83                 db    0
    .data:0040BD84                 db    0
    .data:0040BD85                 db    0
    .data:0040BD86                 db    0
    .data:0040BD87                 db    0
    .data:0040BD88                 db    0
    .data:0040BD89                 db    0
    .data:0040BD8A                 db    0
    .data:0040BD8B                 db    0
    .data:0040BD8C                 db    0
    .data:0040BD8D                 db    0
    .data:0040BD8E                 db    0
    .data:0040BD8F                 db    0
    .data:0040BD90                 db    0
    .data:0040BD91                 db    0
    .data:0040BD92                 db    0
    .data:0040BD93                 db    0
    .data:0040BD94                 db    0
    .data:0040BD95                 db    0
    .data:0040BD96                 db    0
    .data:0040BD97                 db    0
    .data:0040BD98                 db    0
    .data:0040BD99                 db    0
    .data:0040BD9A                 db    0
    .data:0040BD9B                 db    0
    .data:0040BD9C                 db    0
    .data:0040BD9D                 db    0
    .data:0040BD9E                 db    0
    .data:0040BD9F                 db    0
    .data:0040BDA0                 db    0
    .data:0040BDA1                 db    0
    .data:0040BDA2                 db    0
    .data:0040BDA3                 db    0
    .data:0040BDA4                 db    0
    .data:0040BDA5                 db    0
    .data:0040BDA6                 db    0
    .data:0040BDA7                 db    0
    .data:0040BDA8                 db    0
    .data:0040BDA9                 db    0
    .data:0040BDAA                 db    0
    .data:0040BDAB                 db    0
    .data:0040BDAC                 db    0
    .data:0040BDAD                 db    0
    .data:0040BDAE                 db    0
    .data:0040BDAF                 db    0
    .data:0040BDB0                 db    0
    .data:0040BDB1                 db    0
    .data:0040BDB2                 db    0
    .data:0040BDB3                 db    0
    .data:0040BDB4                 db    0
    .data:0040BDB5                 db    0
    .data:0040BDB6                 db    0
    .data:0040BDB7                 db    0
    .data:0040BDB8                 db    0
    .data:0040BDB9                 db    0
    .data:0040BDBA                 db    0
    .data:0040BDBB                 db    0
    .data:0040BDBC                 db    0
    .data:0040BDBD                 db    0
    .data:0040BDBE                 db    0
    .data:0040BDBF                 db    0
    
    .data:0040A508 unk_40A508      db  9Ah ; Ü             ; DATA XREF: _main+62o
    .data:0040A509                 db  2Eh ; .
    .data:0040A50A                 db 0ECh ; 8
    .data:0040A50B                 db  69h ; i
    .data:0040A50C                 db  84h ; ä
    .data:0040A50D                 db    4
    .data:0040A50E                 db  44h ; D
    .data:0040A50F                 db  7Fh ; 
    .data:0040A510                 db    1
    .data:0040A511                 db  15h
    .data:0040A512                 db 0A5h ; Ñ
    .data:0040A513                 db  12h
    .data:0040A514                 db  3Dh ; =
    .data:0040A515                 db  42h ; B
    .data:0040A516                 db  4Fh ; O
    .data:0040A517                 db  0Dh
    .data:0040A518                 db  3Dh ; =
    .data:0040A519                 db  5Ch ; \
    .data:0040A51A                 db  68h ; h
    .data:0040A51B                 db 0A7h ; º
    .data:0040A51C                 db  43h ; C
    .data:0040A51D                 db 0CCh ; ¦
    .data:0040A51E                 db 0C0h ; +
    .data:0040A51F                 db 0D7h ; +
    .data:0040A520                 db  6Eh ; n
    .data:0040A521                 db 0E2h ; G
    .data:0040A522                 db 0DEh ; ¦
    .data:0040A523                 db 0C0h ; +
    .data:0040A524                 db  4Dh ; M
    .data:0040A525                 db 0D5h ; +
    .data:0040A526                 db 0DDh ; ¦
    .data:0040A527                 db 0C6h ; ¦
    .data:0040A528                 db  71h ; q
    .data:0040A529                 db 0DCh ; _
    .data:0040A52A                 db 0D0h ; -
    .data:0040A52B                 db 0C0h ; +
    .data:0040A52C                 db  4Dh ; M
    .data:0040A52D                 db 0D5h ; +
    .data:0040A52E                 db 0DEh ; ¦
    .data:0040A52F                 db 0CFh ; -
    .data:0040A530                 db  7Dh ; }
    .data:0040A531                 db 0DFh ; ¯
    .data:0040A532                 db 0DBh ; ¦
    .data:0040A533                 db 0C0h ; +
    .data:0040A534                 db  6Ah ; j
    .data:0040A535                 db 0D3h ; +
    .data:0040A536                 db 0CEh ; +
    .data:0040A537                 db 0D3h ; +
    .data:0040A538                 db  7Eh ; ~
    .data:0040A539                 db 0DEh ; ¦
    .data:0040A53A                 db 0DFh ; ¯
    .data:0040A53B                 db 0D7h ; +
    .data:0040A53C                 db  68h ; h
    .data:0040A53D                 db 0BEh ; +
    .data:0040A53E                 db 0D4h ; +
    .data:0040A53F                 db 0CFh ; -
    .data:0040A540                 db  78h ; x
    .data:0040A541                 db 0DCh ; _
    .data:0040A542                 db 0CCh ; ¦
    .data:0040A543                 db 0D9h ; +
    .data:0040A544                 db  7Ch ; |
    .data:0040A545                 db 0CFh ; -
    .data:0040A546                 db 0A0h ; á
    .data:0040A547                 db  9Dh ; ¥
    .data:0040A548                 db  3Bh ; ;
    .data:0040A549                 db 0A3h ; ú
    .data:0040A54A                 db  99h ; Ö
    .data:0040A54B                 db 0D4h ; +
    .data:0040A54C                 db  6Dh ; m
    .data:0040A54D                 db 0D6h ; +
    .data:0040A54E                 db  6Bh ; k
    .data:0040A54F                 db 0BDh ; +
    .data:0040A550                 db 0C9h ; +
    .data:0040A551                 db 0B3h ; ¦
    .data:0040A552                 db  56h ; V
    .data:0040A553                 db 0F8h ; °
    .data:0040A554                 db  2Ch ; ,
    .data:0040A555                 db  4Fh ; O
    .data:0040A556                 db  4Fh ; O
    .data:0040A557                 db  7Ah ; z
    .data:0040A558                 db    2
    .data:0040A559                 db  70h ; p
    .data:0040A55A                 db  7Dh ; }
    .data:0040A55B                 db  5Bh ; [
    .data:0040A55C                 db  40h ; @
    .data:0040A55D                 db  38h ; 8
    .data:0040A55E                 db  34h ; 4
    .data:0040A55F                 db  37h ; 7
    .data:0040A560                 db    4
    .data:0040A561                 db 0B4h ; ¦
    .data:0040A562                 db  63h ; c
    .data:0040A563                 db  4Ah ; J
    .data:0040A564                 db 0D6h ; +
    .data:0040A565                 db  5Eh ; ^
    .data:0040A566                 db  1Eh
    .data:0040A567                 db  8Ch ; î
    .data:0040A568                 db 0DDh ; ¦
    .data:0040A569                 db  5Bh ; [
    .data:0040A56A                 db  72h ; r
    .data:0040A56B                 db  20h
    .data:0040A56C                 db 0A8h ; ¿
    .data:0040A56D                 db 0E5h ; s
    .data:0040A56E                 db 0BCh ; +
    .data:0040A56F                 db  88h ; ê
    .data:0040A570                 db  8Fh ; Å
    .data:0040A571                 db  7Bh ; {
    .data:0040A572                 db  2Dh ; -
    .data:0040A573                 db 0FCh ; n
    .data:0040A574                 db  5Bh ; [
    .data:0040A575                 db 0BAh ; ¦
    .data:0040A576                 db 0BDh ; +
    .data:0040A577                 db  4Ah ; J
    .data:0040A578                 db 0A4h ; ñ
    .data:0040A579                 db  8Fh ; Å
    .data:0040A57A                 db 0BCh ; +
    .data:0040A57B                 db  16h
    .data:0040A57C                 db  27h ; '
    .data:0040A57D                 db  99h ; Ö
    .data:0040A57E                 db 0AAh ; ¬
    .data:0040A57F                 db 0FBh ; v
    .data:0040A580                 db 0E9h ; T
    .data:0040A581                 db  67h ; g
    .data:0040A582                 db  19h
    .data:0040A583                 db 0D0h ; -
    .data:0040A584                 db  8Fh ; Å
    .data:0040A585                 db 0EFh ; n
    .data:0040A586                 db 0CCh ; ¦
    .data:0040A587                 db  8Dh ; ì
    .data:0040A588                 db  25h ; %
    .data:0040A589                 db 0EEh ; e
    .data:0040A58A                 db 0B7h ; +
    .data:0040A58B                 db  24h ; $
    .data:0040A58C                 db  2Eh ; .
    .data:0040A58D                 db    6
    .data:0040A58E                 db  2Ch ; ,
    .data:0040A58F                 db  44h ; D
    .data:0040A590                 db  6Ah ; j
    .data:0040A591                 db 0C2h ; -
    .data:0040A592                 db 0CCh ; ¦
    .data:0040A593                 db  53h ; S
    .data:0040A594                 db  7Eh ; ~
    .data:0040A595                 db  7Ah ; z
    .data:0040A596                 db  98h ; ÿ
    .data:0040A597                 db  9Ch ; £
    .data:0040A598                 db 0F3h ; =
    .data:0040A599                 db  11h
    .data:0040A59A                 db 0A2h ; ó
    .data:0040A59B                 db 0F9h ; ·
    .data:0040A59C                 db 0CDh ; -
    .data:0040A59D                 db  14h
    .data:0040A59E                 db  46h ; F
    .data:0040A59F                 db 0FCh ; n
    .data:0040A5A0                 db  16h
    .data:0040A5A1                 db 0D3h ; +
    .data:0040A5A2                 db  77h ; w
    .data:0040A5A3                 db  60h ; `
    .data:0040A5A4                 db  2Eh ; .
    .data:0040A5A5                 db 0D6h ; +
    .data:0040A5A6                 db  74h ; t
    .data:0040A5A7                 db  35h ; 5
    .data:0040A5A8                 db 0BAh ; ¦
    .data:0040A5A9                 db 0CEh ; +
    .data:0040A5AA                 db 0F4h ; (
    .data:0040A5AB                 db 0A7h ; º
    .data:0040A5AC                 db  7Bh ; {
    .data:0040A5AD                 db  75h ; u
    .data:0040A5AE                 db 0ABh ; ½
    .data:0040A5AF                 db  4Bh ; K
    .data:0040A5B0                 db 0EEh ; e
    .data:0040A5B1                 db  6Bh ; k
    .data:0040A5B2                 db 0AAh ; ¬
    .data:0040A5B3                 db  3Dh ; =
    .data:0040A5B4                 db 0F6h ; ÷
    .data:0040A5B5                 db  0Eh
    .data:0040A5B6                 db  84h ; ä
    .data:0040A5B7                 db  1Fh
    .data:0040A5B8                 db  84h ; ä
    .data:0040A5B9                 db 0D5h ; +
    .data:0040A5BA                 db 0ABh ; ½
    .data:0040A5BB                 db 0A9h ; ¬
    .data:0040A5BC                 db 0E6h ; µ
    .data:0040A5BD                 db  32h ; 2
    .data:0040A5BE                 db    6
    .data:0040A5BF                 db 0DDh ; ¦
    .data:0040A5C0                 db 0BFh ; +
    .data:0040A5C1                 db 0F6h ; ÷
    .data:0040A5C2                 db  25h ; %
    .data:0040A5C3                 db 0A2h ; ó
    .data:0040A5C4                 db  52h ; R
    .data:0040A5C5                 db  4Ah ; J
    .data:0040A5C6                 db  0Eh
    .data:0040A5C7                 db 0BCh ; +
    .data:0040A5C8                 db  15h
    .data:0040A5C9                 db  36h ; 6
    .data:0040A5CA                 db  9Ah ; Ü
    .data:0040A5CB                 db 0F8h ; °
    .data:0040A5CC                 db 0C5h ; +
    .data:0040A5CD                 db 0BAh ; ¦
    .data:0040A5CE                 db  4Ch ; L
    .data:0040A5CF                 db  0Ah
    .data:0040A5D0                 db 0F3h ; =
    .data:0040A5D1                 db  8Dh ; ì
    .data:0040A5D2                 db 0A2h ; ó
    .data:0040A5D3                 db  4Eh ; N
    .data:0040A5D4                 db 0A9h ; ¬
    .data:0040A5D5                 db  65h ; e
    .data:0040A5D6                 db  4Ah ; J
    .data:0040A5D7                 db  95h ; ò
    .data:0040A5D8                 db  2Fh ; /
    .data:0040A5D9                 db  72h ; r
    .data:0040A5DA                 db 0BBh ; +
    .data:0040A5DB                 db  9Eh ; P
    .data:0040A5DC                 db  28h ; (
    .data:0040A5DD                 db 0F4h ; (
    .data:0040A5DE                 db  0Dh
    .data:0040A5DF                 db  55h ; U
    .data:0040A5E0                 db 0E0h ; a
    .data:0040A5E1                 db    3
    .data:0040A5E2                 db  2Dh ; -
    .data:0040A5E3                 db  15h
    .data:0040A5E4                 db  25h ; %
    .data:0040A5E5                 db  77h ; w
    .data:0040A5E6                 db 0B5h ; ¦
    .data:0040A5E7                 db 0EEh ; e
    .data:0040A5E8                 db 0EEh ; e
    .data:0040A5E9                 db  92h ; Æ
    .data:0040A5EA                 db  7Dh ; }
    .data:0040A5EB                 db 0BCh ; +
    .data:0040A5EC                 db  44h ; D
    .data:0040A5ED                 db 0CDh ; -
    .data:0040A5EE                 db  43h ; C
    .data:0040A5EF                 db    4
    .data:0040A5F0                 db  97h ; ù
    .data:0040A5F1                 db 0F5h ; )
    .data:0040A5F2                 db 0EEh ; e
    .data:0040A5F3                 db 0EEh ; e
    .data:0040A5F4                 db  7Eh ; ~
    .data:0040A5F5                 db  67h ; g
    .data:0040A5F6                 db  5Ah ; Z
    .data:0040A5F7                 db 0D4h ; +
    .data:0040A5F8                 db  91h ; æ
    .data:0040A5F9                 db  2Fh ; /
    .data:0040A5FA                 db  97h ; ù
    .data:0040A5FB                 db  24h ; $
    .data:0040A5FC                 db 0C9h ; +
    .data:0040A5FD                 db  4Ch ; L
    .data:0040A5FE                 db  22h ; "
    .data:0040A5FF                 db  2Eh ; .
    .data:0040A600                 db  37h ; 7
    .data:0040A601                 db 0DDh ; ¦
    .data:0040A602                 db 0FEh ; ¦
    .data:0040A603                 db  89h ; ë
    .data:0040A604                 db 0CFh ; -
    .data:0040A605                 db 0FDh ; ²
    .data:0040A606                 db  29h ; )
    .data:0040A607                 db    0
    
    .data:0040BDC0 unk_40BDC0      db    0                 ; DATA XREF: _main+5Do
    .data:0040BDC1                 db    0
    .data:0040BDC2                 db    0
    .data:0040BDC3                 db    0
    .data:0040BDC4                 db    0
    .data:0040BDC5                 db    0
    .data:0040BDC6                 db    0
    .data:0040BDC7                 db    0
    .data:0040BDC8                 db    0
    .data:0040BDC9                 db    0
    .data:0040BDCA                 db    0
    .data:0040BDCB                 db    0
    .data:0040BDCC                 db    0
    .data:0040BDCD                 db    0
    .data:0040BDCE                 db    0
    .data:0040BDCF                 db    0
    .data:0040BDD0                 db    0
    .data:0040BDD1                 db    0
    .data:0040BDD2                 db    0
    .data:0040BDD3                 db    0
    .data:0040BDD4                 db    0
    .data:0040BDD5                 db    0
    .data:0040BDD6                 db    0
    .data:0040BDD7                 db    0
    .data:0040BDD8                 db    0
    .data:0040BDD9                 db    0
    .data:0040BDDA                 db    0
    .data:0040BDDB                 db    0
    .data:0040BDDC                 db    0
    .data:0040BDDD                 db    0
    .data:0040BDDE                 db    0
    .data:0040BDDF                 db    0
    .data:0040BDE0                 db    0
    .data:0040BDE1                 db    0
    .data:0040BDE2                 db    0
    .data:0040BDE3                 db    0
    .data:0040BDE4                 db    0
    .data:0040BDE5                 db    0
    .data:0040BDE6                 db    0
    .data:0040BDE7                 db    0
    .data:0040BDE8                 db    0
    .data:0040BDE9                 db    0
    .data:0040BDEA                 db    0
    .data:0040BDEB                 db    0
    .data:0040BDEC                 db    0
    .data:0040BDED                 db    0
    .data:0040BDEE                 db    0
    .data:0040BDEF                 db    0
    .data:0040BDF0                 db    0
    .data:0040BDF1                 db    0
    .data:0040BDF2                 db    0
    .data:0040BDF3                 db    0
    .data:0040BDF4                 db    0
    .data:0040BDF5                 db    0
    .data:0040BDF6                 db    0
    .data:0040BDF7                 db    0
    .data:0040BDF8                 db    0
    .data:0040BDF9                 db    0
    .data:0040BDFA                 db    0
    .data:0040BDFB                 db    0
    .data:0040BDFC                 db    0
    .data:0040BDFD                 db    0
    .data:0040BDFE                 db    0
    .data:0040BDFF                 db    0
    .data:0040BE00                 db    0
    .data:0040BE01                 db    0
    .data:0040BE02                 db    0
    .data:0040BE03                 db    0
    .data:0040BE04                 db    0
    .data:0040BE05                 db    0
    .data:0040BE06                 db    0
    .data:0040BE07                 db    0
    .data:0040BE08                 db    0
    .data:0040BE09                 db    0
    .data:0040BE0A                 db    0
    .data:0040BE0B                 db    0
    .data:0040BE0C                 db    0
    .data:0040BE0D                 db    0
    .data:0040BE0E                 db    0
    .data:0040BE0F                 db    0
    .data:0040BE10                 db    0
    .data:0040BE11                 db    0
    .data:0040BE12                 db    0
    .data:0040BE13                 db    0
    .data:0040BE14                 db    0
    .data:0040BE15                 db    0
    .data:0040BE16                 db    0
    .data:0040BE17                 db    0
    .data:0040BE18                 db    0
    .data:0040BE19                 db    0
    .data:0040BE1A                 db    0
    .data:0040BE1B                 db    0
    .data:0040BE1C                 db    0
    .data:0040BE1D                 db    0
    .data:0040BE1E                 db    0
    .data:0040BE1F                 db    0
    .data:0040BE20                 db    0
    .data:0040BE21                 db    0
    .data:0040BE22                 db    0
    .data:0040BE23                 db    0
    .data:0040BE24                 db    0
    .data:0040BE25                 db    0
    .data:0040BE26                 db    0
    .data:0040BE27                 db    0
    .data:0040BE28                 db    0
    .data:0040BE29                 db    0
    .data:0040BE2A                 db    0
    .data:0040BE2B                 db    0
    .data:0040BE2C                 db    0
    .data:0040BE2D                 db    0
    .data:0040BE2E                 db    0
    .data:0040BE2F                 db    0
    .data:0040BE30                 db    0
    .data:0040BE31                 db    0
    .data:0040BE32                 db    0
    .data:0040BE33                 db    0
    .data:0040BE34                 db    0
    .data:0040BE35                 db    0
    .data:0040BE36                 db    0
    .data:0040BE37                 db    0
    .data:0040BE38                 db    0
    .data:0040BE39                 db    0
    .data:0040BE3A                 db    0
    .data:0040BE3B                 db    0
    .data:0040BE3C                 db    0
    .data:0040BE3D                 db    0
    .data:0040BE3E                 db    0
    .data:0040BE3F                 db    0
    .data:0040BE40                 db    0
    .data:0040BE41                 db    0
    .data:0040BE42                 db    0
    .data:0040BE43                 db    0
    .data:0040BE44                 db    0
    .data:0040BE45                 db    0
    .data:0040BE46                 db    0
    .data:0040BE47                 db    0
    .data:0040BE48                 db    0
    .data:0040BE49                 db    0
    .data:0040BE4A                 db    0
    .data:0040BE4B                 db    0
    .data:0040BE4C                 db    0
    .data:0040BE4D                 db    0
    .data:0040BE4E                 db    0
    .data:0040BE4F                 db    0
    .data:0040BE50                 db    0
    .data:0040BE51                 db    0
    .data:0040BE52                 db    0
    .data:0040BE53                 db    0
    .data:0040BE54                 db    0
    .data:0040BE55                 db    0
    .data:0040BE56                 db    0
    .data:0040BE57                 db    0
    .data:0040BE58                 db    0
    .data:0040BE59                 db    0
    .data:0040BE5A                 db    0
    .data:0040BE5B                 db    0
    .data:0040BE5C                 db    0
    .data:0040BE5D                 db    0
    .data:0040BE5E                 db    0
    .data:0040BE5F                 db    0
    .data:0040BE60                 db    0
    .data:0040BE61                 db    0
    .data:0040BE62                 db    0
    .data:0040BE63                 db    0
    .data:0040BE64                 db    0
    .data:0040BE65                 db    0
    .data:0040BE66                 db    0
    .data:0040BE67                 db    0
    .data:0040BE68                 db    0
    .data:0040BE69                 db    0
    .data:0040BE6A                 db    0
    .data:0040BE6B                 db    0
    .data:0040BE6C                 db    0
    .data:0040BE6D                 db    0
    .data:0040BE6E                 db    0
    .data:0040BE6F                 db    0
    .data:0040BE70                 db    0
    .data:0040BE71                 db    0
    .data:0040BE72                 db    0
    .data:0040BE73                 db    0
    .data:0040BE74                 db    0
    .data:0040BE75                 db    0
    .data:0040BE76                 db    0
    .data:0040BE77                 db    0
    .data:0040BE78                 db    0
    .data:0040BE79                 db    0
    .data:0040BE7A                 db    0
    .data:0040BE7B                 db    0
    .data:0040BE7C                 db    0
    .data:0040BE7D                 db    0
    .data:0040BE7E                 db    0
    .data:0040BE7F                 db    0
    .data:0040BE80                 db    0
    .data:0040BE81                 db    0
    .data:0040BE82                 db    0
    .data:0040BE83                 db    0
    .data:0040BE84                 db    0
    .data:0040BE85                 db    0
    .data:0040BE86                 db    0
    .data:0040BE87                 db    0
    .data:0040BE88                 db    0
    .data:0040BE89                 db    0
    .data:0040BE8A                 db    0
    .data:0040BE8B                 db    0
    .data:0040BE8C                 db    0
    .data:0040BE8D                 db    0
    .data:0040BE8E                 db    0
    .data:0040BE8F                 db    0
    .data:0040BE90                 db    0
    .data:0040BE91                 db    0
    .data:0040BE92                 db    0
    .data:0040BE93                 db    0
    .data:0040BE94                 db    0
    .data:0040BE95                 db    0
    .data:0040BE96                 db    0
    .data:0040BE97                 db    0
    .data:0040BE98                 db    0
    .data:0040BE99                 db    0
    .data:0040BE9A                 db    0
    .data:0040BE9B                 db    0
    .data:0040BE9C                 db    0
    .data:0040BE9D                 db    0
    .data:0040BE9E                 db    0
    .data:0040BE9F                 db    0
    .data:0040BEA0                 db    0
    .data:0040BEA1                 db    0
    .data:0040BEA2                 db    0
    .data:0040BEA3                 db    0
    .data:0040BEA4                 db    0
    .data:0040BEA5                 db    0
    .data:0040BEA6                 db    0
    .data:0040BEA7                 db    0
    .data:0040BEA8                 db    0
    .data:0040BEA9                 db    0
    .data:0040BEAA                 db    0
    .data:0040BEAB                 db    0
    .data:0040BEAC                 db    0
    .data:0040BEAD                 db    0
    .data:0040BEAE                 db    0
    .data:0040BEAF                 db    0
    .data:0040BEB0                 db    0
    .data:0040BEB1                 db    0
    .data:0040BEB2                 db    0
    .data:0040BEB3                 db    0
    .data:0040BEB4                 db    0
    .data:0040BEB5                 db    0
    .data:0040BEB6                 db    0
    .data:0040BEB7                 db    0
    .data:0040BEB8                 db    0
    .data:0040BEB9                 db    0
    .data:0040BEBA                 db    0
    .data:0040BEBB                 db    0
    .data:0040BEBC                 db    0
    .data:0040BEBD                 db    0
    .data:0040BEBE                 db    0
    .data:0040BEBF                 db    0
    .data:0040BEC0                 db    0
    .data:0040BEC1                 db    0
    .data:0040BEC2                 db    0
    .data:0040BEC3                 db    0
    .data:0040BEC4                 db    0
    .data:0040BEC5                 db    0
    .data:0040BEC6                 db    0
    .data:0040BEC7                 db    0
    .data:0040BEC8                 db    0
    .data:0040BEC9                 db    0
    .data:0040BECA                 db    0
    .data:0040BECB                 db    0
    .data:0040BECC                 db    0
    .data:0040BECD                 db    0
    .data:0040BECE                 db    0
    .data:0040BECF                 db    0
    .data:0040BED0                 db    0
    .data:0040BED1                 db    0
    .data:0040BED2                 db    0
    .data:0040BED3                 db    0
    .data:0040BED4                 db    0
    .data:0040BED5                 db    0
    .data:0040BED6                 db    0
    .data:0040BED7                 db    0
    .data:0040BED8                 db    0
    .data:0040BED9                 db    0
    .data:0040BEDA                 db    0
    .data:0040BEDB                 db    0
    .data:0040BEDC                 db    0
    .data:0040BEDD                 db    0
    .data:0040BEDE                 db    0
    .data:0040BEDF                 db    0
    .data:0040BEE0                 db    0
    .data:0040BEE1                 db    0
    .data:0040BEE2                 db    0
    .data:0040BEE3                 db    0
    .data:0040BEE4                 db    0
    .data:0040BEE5                 db    0
    .data:0040BEE6                 db    0
    .data:0040BEE7                 db    0
    .data:0040BEE8                 db    0
    .data:0040BEE9                 db    0
    .data:0040BEEA                 db    0
    .data:0040BEEB                 db    0
    .data:0040BEEC                 db    0
    .data:0040BEED                 db    0
    .data:0040BEEE                 db    0
    .data:0040BEEF                 db    0
    .data:0040BEF0                 db    0
    .data:0040BEF1                 db    0
    .data:0040BEF2                 db    0
    .data:0040BEF3                 db    0
    .data:0040BEF4                 db    0
    .data:0040BEF5                 db    0
    .data:0040BEF6                 db    0
    .data:0040BEF7                 db    0
    .data:0040BEF8                 db    0
    .data:0040BEF9                 db    0
    .data:0040BEFA                 db    0
    .data:0040BEFB                 db    0
    .data:0040BEFC                 db    0
    .data:0040BEFD                 db    0
    .data:0040BEFE                 db    0
    .data:0040BEFF                 db    0
    .data:0040BF00                 db    0
    .data:0040BF01                 db    0
    .data:0040BF02                 db    0
    .data:0040BF03                 db    0
    .data:0040BF04                 db    0
    .data:0040BF05                 db    0
    .data:0040BF06                 db    0
    .data:0040BF07                 db    0
    .data:0040BF08                 db    0
    .data:0040BF09                 db    0
    .data:0040BF0A                 db    0
    .data:0040BF0B                 db    0
    .data:0040BF0C                 db    0
    .data:0040BF0D                 db    0
    .data:0040BF0E                 db    0
    .data:0040BF0F                 db    0
    .data:0040BF10                 db    0
    .data:0040BF11                 db    0
    .data:0040BF12                 db    0
    .data:0040BF13                 db    0
    .data:0040BF14                 db    0
    .data:0040BF15                 db    0
    .data:0040BF16                 db    0
    .data:0040BF17                 db    0
    .data:0040BF18                 db    0
    .data:0040BF19                 db    0
    .data:0040BF1A                 db    0
    .data:0040BF1B                 db    0
    .data:0040BF1C                 db    0
    .data:0040BF1D                 db    0
    .data:0040BF1E                 db    0
    .data:0040BF1F                 db    0
    .data:0040BF20                 db    0
    .data:0040BF21                 db    0
    .data:0040BF22                 db    0
    .data:0040BF23                 db    0
    .data:0040BF24                 db    0
    .data:0040BF25                 db    0
    .data:0040BF26                 db    0
    .data:0040BF27                 db    0
    .data:0040BF28                 db    0
    .data:0040BF29                 db    0
    .data:0040BF2A                 db    0
    .data:0040BF2B                 db    0
    .data:0040BF2C                 db    0
    .data:0040BF2D                 db    0
    .data:0040BF2E                 db    0
    .data:0040BF2F                 db    0
    .data:0040BF30                 db    0
    .data:0040BF31                 db    0
    .data:0040BF32                 db    0
    .data:0040BF33                 db    0
    .data:0040BF34                 db    0
    .data:0040BF35                 db    0
    .data:0040BF36                 db    0
    .data:0040BF37                 db    0
    .data:0040BF38                 db    0
    .data:0040BF39                 db    0
    .data:0040BF3A                 db    0
    .data:0040BF3B                 db    0
    .data:0040BF3C                 db    0
    .data:0040BF3D                 db    0
    .data:0040BF3E                 db    0
    .data:0040BF3F                 db    0
    .data:0040BF40                 db    0
    .data:0040BF41                 db    0
    .data:0040BF42                 db    0
    .data:0040BF43                 db    0
    .data:0040BF44                 db    0
    .data:0040BF45                 db    0
    .data:0040BF46                 db    0
    .data:0040BF47                 db    0
    .data:0040BF48                 db    0
    .data:0040BF49                 db    0
    .data:0040BF4A                 db    0
    .data:0040BF4B                 db    0
    .data:0040BF4C                 db    0
    .data:0040BF4D                 db    0
    .data:0040BF4E                 db    0
    .data:0040BF4F                 db    0
    .data:0040BF50                 db    0
    .data:0040BF51                 db    0
    .data:0040BF52                 db    0
    .data:0040BF53                 db    0
    .data:0040BF54                 db    0
    .data:0040BF55                 db    0
    .data:0040BF56                 db    0
    .data:0040BF57                 db    0
    .data:0040BF58                 db    0
    .data:0040BF59                 db    0
    .data:0040BF5A                 db    0
    .data:0040BF5B                 db    0
    .data:0040BF5C                 db    0
    .data:0040BF5D                 db    0
    .data:0040BF5E                 db    0
    .data:0040BF5F                 db    0
    .data:0040BF60                 db    0
    .data:0040BF61                 db    0
    .data:0040BF62                 db    0
    .data:0040BF63                 db    0
    .data:0040BF64                 db    0
    .data:0040BF65                 db    0
    .data:0040BF66                 db    0
    .data:0040BF67                 db    0
    .data:0040BF68                 db    0
    .data:0040BF69                 db    0
    .data:0040BF6A                 db    0
    .data:0040BF6B                 db    0
    .data:0040BF6C                 db    0
    .data:0040BF6D                 db    0
    .data:0040BF6E                 db    0
    .data:0040BF6F                 db    0
    .data:0040BF70                 db    0
    .data:0040BF71                 db    0
    .data:0040BF72                 db    0
    .data:0040BF73                 db    0
    .data:0040BF74                 db    0
    .data:0040BF75                 db    0
    .data:0040BF76                 db    0
    .data:0040BF77                 db    0
    .data:0040BF78                 db    0
    .data:0040BF79                 db    0
    .data:0040BF7A                 db    0
    .data:0040BF7B                 db    0
    .data:0040BF7C                 db    0
    .data:0040BF7D                 db    0
    .data:0040BF7E                 db    0
    .data:0040BF7F                 db    0
    .data:0040BF80                 db    0
    .data:0040BF81                 db    0
    .data:0040BF82                 db    0
    .data:0040BF83                 db    0
    .data:0040BF84                 db    0
    .data:0040BF85                 db    0
    .data:0040BF86                 db    0
    .data:0040BF87                 db    0
    .data:0040BF88                 db    0
    .data:0040BF89                 db    0
    .data:0040BF8A                 db    0
    .data:0040BF8B                 db    0
    .data:0040BF8C                 db    0
    .data:0040BF8D                 db    0
    .data:0040BF8E                 db    0
    .data:0040BF8F                 db    0
    .data:0040BF90                 db    0
    .data:0040BF91                 db    0
    .data:0040BF92                 db    0
    .data:0040BF93                 db    0
    .data:0040BF94                 db    0
    .data:0040BF95                 db    0
    .data:0040BF96                 db    0
    .data:0040BF97                 db    0
    .data:0040BF98                 db    0
    .data:0040BF99                 db    0
    .data:0040BF9A                 db    0
    .data:0040BF9B                 db    0
    .data:0040BF9C                 db    0
    .data:0040BF9D                 db    0
    .data:0040BF9E                 db    0
    .data:0040BF9F                 db    0
    .data:0040BFA0                 db    0
    .data:0040BFA1                 db    0
    .data:0040BFA2                 db    0
    .data:0040BFA3                 db    0
    .data:0040BFA4                 db    0
    .data:0040BFA5                 db    0
    .data:0040BFA6                 db    0
    .data:0040BFA7                 db    0
    .data:0040BFA8                 db    0
    .data:0040BFA9                 db    0
    .data:0040BFAA                 db    0
    .data:0040BFAB                 db    0
    .data:0040BFAC                 db    0
    .data:0040BFAD                 db    0
    .data:0040BFAE                 db    0
    .data:0040BFAF                 db    0
    .data:0040BFB0                 db    0
    .data:0040BFB1                 db    0
    .data:0040BFB2                 db    0
    .data:0040BFB3                 db    0
    .data:0040BFB4                 db    0
    .data:0040BFB5                 db    0
    .data:0040BFB6                 db    0
    .data:0040BFB7                 db    0
    .data:0040BFB8                 db    0
    .data:0040BFB9                 db    0
    .data:0040BFBA                 db    0
    .data:0040BFBB                 db    0
    .data:0040BFBC                 db    0
    .data:0040BFBD                 db    0
    .data:0040BFBE                 db    0
    .data:0040BFBF                 db    0
    
    .data:0040C1C0 ; const WCHAR szRemoteFile
    .data:0040C1C0 szRemoteFile    dw ?                    ; DATA XREF: sub_401080+58o
    .data:0040C1C0                                         ; sub_401080+5Do ...
    .data:0040C1C2                 db    ? ;
    .data:0040C1C3                 db    ? ;
    .data:0040C1C4                 db    ? ;
    .data:0040C1C5                 db    ? ;
    .data:0040C1C6                 db    ? ;
    .data:0040C1C7                 db    ? ;
    .data:0040C1C8                 db    ? ;
    .data:0040C1C9                 db    ? ;
    .data:0040C1CA                 db    ? ;
    .data:0040C1CB                 db    ? ;
    .data:0040C1CC                 db    ? ;
    .data:0040C1CD                 db    ? ;
    .data:0040C1CE                 db    ? ;
    .data:0040C1CF                 db    ? ;
    .data:0040C1D0                 db    ? ;
    .data:0040C1D1                 db    ? ;
    .data:0040C1D2                 db    ? ;
    .data:0040C1D3                 db    ? ;
    .data:0040C1D4                 db    ? ;
    .data:0040C1D5                 db    ? ;
    .data:0040C1D6                 db    ? ;
    .data:0040C1D7                 db    ? ;
    .data:0040C1D8                 db    ? ;
    .data:0040C1D9                 db    ? ;
    .data:0040C1DA                 db    ? ;
    .data:0040C1DB                 db    ? ;
    .data:0040C1DC                 db    ? ;
    .data:0040C1DD                 db    ? ;
    .data:0040C1DE                 db    ? ;
    .data:0040C1DF                 db    ? ;
    .data:0040C1E0                 db    ? ;
    .data:0040C1E1                 db    ? ;
    .data:0040C1E2                 db    ? ;
    .data:0040C1E3                 db    ? ;
    .data:0040C1E4                 db    ? ;
    .data:0040C1E5                 db    ? ;
    .data:0040C1E6                 db    ? ;
    .data:0040C1E7                 db    ? ;
    .data:0040C1E8                 db    ? ;
    .data:0040C1E9                 db    ? ;
    .data:0040C1EA                 db    ? ;
    .data:0040C1EB                 db    ? ;
    .data:0040C1EC                 db    ? ;
    .data:0040C1ED                 db    ? ;
    .data:0040C1EE                 db    ? ;
    .data:0040C1EF                 db    ? ;
    .data:0040C1F0                 db    ? ;
    .data:0040C1F1                 db    ? ;
    .data:0040C1F2                 db    ? ;
    .data:0040C1F3                 db    ? ;
    .data:0040C1F4                 db    ? ;
    .data:0040C1F5                 db    ? ;
    .data:0040C1F6                 db    ? ;
    .data:0040C1F7                 db    ? ;
    .data:0040C1F8                 db    ? ;
    .data:0040C1F9                 db    ? ;
    .data:0040C1FA                 db    ? ;
    .data:0040C1FB                 db    ? ;
    .data:0040C1FC                 db    ? ;
    .data:0040C1FD                 db    ? ;
    .data:0040C1FE                 db    ? ;
    .data:0040C1FF                 db    ? ;
    .data:0040C200                 db    ? ;
    .data:0040C201                 db    ? ;
    .data:0040C202                 db    ? ;
    .data:0040C203                 db    ? ;
    .data:0040C204                 db    ? ;
    .data:0040C205                 db    ? ;
    .data:0040C206                 db    ? ;
    .data:0040C207                 db    ? ;
    .data:0040C208                 db    ? ;
    .data:0040C209                 db    ? ;
    .data:0040C20A                 db    ? ;
    .data:0040C20B                 db    ? ;
    .data:0040C20C                 db    ? ;
    .data:0040C20D                 db    ? ;
    .data:0040C20E                 db    ? ;
    .data:0040C20F                 db    ? ;
    .data:0040C210                 db    ? ;
    .data:0040C211                 db    ? ;
    .data:0040C212                 db    ? ;
    .data:0040C213                 db    ? ;
    .data:0040C214                 db    ? ;
    .data:0040C215                 db    ? ;
    .data:0040C216                 db    ? ;
    .data:0040C217                 db    ? ;
    .data:0040C218                 db    ? ;
    .data:0040C219                 db    ? ;
    .data:0040C21A                 db    ? ;
    .data:0040C21B                 db    ? ;
    .data:0040C21C                 db    ? ;
    .data:0040C21D                 db    ? ;
    .data:0040C21E                 db    ? ;
    .data:0040C21F                 db    ? ;
    .data:0040C220                 db    ? ;
    .data:0040C221                 db    ? ;
    .data:0040C222                 db    ? ;
    .data:0040C223                 db    ? ;
    .data:0040C224                 db    ? ;
    .data:0040C225                 db    ? ;
    .data:0040C226                 db    ? ;
    .data:0040C227                 db    ? ;
    .data:0040C228                 db    ? ;
    .data:0040C229                 db    ? ;
    .data:0040C22A                 db    ? ;
    .data:0040C22B                 db    ? ;
    .data:0040C22C                 db    ? ;
    .data:0040C22D                 db    ? ;
    .data:0040C22E                 db    ? ;
    .data:0040C22F                 db    ? ;
    .data:0040C230                 db    ? ;
    .data:0040C231                 db    ? ;
    .data:0040C232                 db    ? ;
    .data:0040C233                 db    ? ;
    .data:0040C234                 db    ? ;
    .data:0040C235                 db    ? ;
    .data:0040C236                 db    ? ;
    .data:0040C237                 db    ? ;
    .data:0040C238                 db    ? ;
    .data:0040C239                 db    ? ;
    .data:0040C23A                 db    ? ;
    .data:0040C23B                 db    ? ;
    .data:0040C23C                 db    ? ;
    .data:0040C23D                 db    ? ;
    .data:0040C23E                 db    ? ;
    .data:0040C23F                 db    ? ;
    .data:0040C240                 db    ? ;
    .data:0040C241                 db    ? ;
    .data:0040C242                 db    ? ;
    .data:0040C243                 db    ? ;
    .data:0040C244                 db    ? ;
    .data:0040C245                 db    ? ;
    .data:0040C246                 db    ? ;
    .data:0040C247                 db    ? ;
    .data:0040C248                 db    ? ;
    .data:0040C249                 db    ? ;
    .data:0040C24A                 db    ? ;
    .data:0040C24B                 db    ? ;
    .data:0040C24C                 db    ? ;
    .data:0040C24D                 db    ? ;
    .data:0040C24E                 db    ? ;
    .data:0040C24F                 db    ? ;
    .data:0040C250                 db    ? ;
    .data:0040C251                 db    ? ;
    .data:0040C252                 db    ? ;
    .data:0040C253                 db    ? ;
    .data:0040C254                 db    ? ;
    .data:0040C255                 db    ? ;
    .data:0040C256                 db    ? ;
    .data:0040C257                 db    ? ;
    .data:0040C258                 db    ? ;
    .data:0040C259                 db    ? ;
    .data:0040C25A                 db    ? ;
    .data:0040C25B                 db    ? ;
    .data:0040C25C                 db    ? ;
    .data:0040C25D                 db    ? ;
    .data:0040C25E                 db    ? ;
    .data:0040C25F                 db    ? ;
    .data:0040C260                 db    ? ;
    .data:0040C261                 db    ? ;
    .data:0040C262                 db    ? ;
    .data:0040C263                 db    ? ;
    .data:0040C264                 db    ? ;
    .data:0040C265                 db    ? ;
    .data:0040C266                 db    ? ;
    .data:0040C267                 db    ? ;
    .data:0040C268                 db    ? ;
    .data:0040C269                 db    ? ;
    .data:0040C26A                 db    ? ;
    .data:0040C26B                 db    ? ;
    .data:0040C26C                 db    ? ;
    .data:0040C26D                 db    ? ;
    .data:0040C26E                 db    ? ;
    .data:0040C26F                 db    ? ;
    .data:0040C270                 db    ? ;
    .data:0040C271                 db    ? ;
    .data:0040C272                 db    ? ;
    .data:0040C273                 db    ? ;
    .data:0040C274                 db    ? ;
    .data:0040C275                 db    ? ;
    .data:0040C276                 db    ? ;
    .data:0040C277                 db    ? ;
    .data:0040C278                 db    ? ;
    .data:0040C279                 db    ? ;
    .data:0040C27A                 db    ? ;
    .data:0040C27B                 db    ? ;
    .data:0040C27C                 db    ? ;
    .data:0040C27D                 db    ? ;
    .data:0040C27E                 db    ? ;
    .data:0040C27F                 db    ? ;
    .data:0040C280                 db    ? ;
    .data:0040C281                 db    ? ;
    .data:0040C282                 db    ? ;
    .data:0040C283                 db    ? ;
    .data:0040C284                 db    ? ;
    .data:0040C285                 db    ? ;
    .data:0040C286                 db    ? ;
    .data:0040C287                 db    ? ;
    .data:0040C288                 db    ? ;
    .data:0040C289                 db    ? ;
    .data:0040C28A                 db    ? ;
    .data:0040C28B                 db    ? ;
    .data:0040C28C                 db    ? ;
    .data:0040C28D                 db    ? ;
    .data:0040C28E                 db    ? ;
    .data:0040C28F                 db    ? ;
    .data:0040C290                 db    ? ;
    .data:0040C291                 db    ? ;
    .data:0040C292                 db    ? ;
    .data:0040C293                 db    ? ;
    .data:0040C294                 db    ? ;
    .data:0040C295                 db    ? ;
    .data:0040C296                 db    ? ;
    .data:0040C297                 db    ? ;
    .data:0040C298                 db    ? ;
    .data:0040C299                 db    ? ;
    .data:0040C29A                 db    ? ;
    .data:0040C29B                 db    ? ;
    .data:0040C29C                 db    ? ;
    .data:0040C29D                 db    ? ;
    .data:0040C29E                 db    ? ;
    .data:0040C29F                 db    ? ;
    .data:0040C2A0                 db    ? ;
    .data:0040C2A1                 db    ? ;
    .data:0040C2A2                 db    ? ;
    .data:0040C2A3                 db    ? ;
    .data:0040C2A4                 db    ? ;
    .data:0040C2A5                 db    ? ;
    .data:0040C2A6                 db    ? ;
    .data:0040C2A7                 db    ? ;
    .data:0040C2A8                 db    ? ;
    .data:0040C2A9                 db    ? ;
    .data:0040C2AA                 db    ? ;
    .data:0040C2AB                 db    ? ;
    .data:0040C2AC                 db    ? ;
    .data:0040C2AD                 db    ? ;
    .data:0040C2AE                 db    ? ;
    .data:0040C2AF                 db    ? ;
    .data:0040C2B0                 db    ? ;
    .data:0040C2B1                 db    ? ;
    .data:0040C2B2                 db    ? ;
    .data:0040C2B3                 db    ? ;
    .data:0040C2B4                 db    ? ;
    .data:0040C2B5                 db    ? ;
    .data:0040C2B6                 db    ? ;
    .data:0040C2B7                 db    ? ;
    .data:0040C2B8                 db    ? ;
    .data:0040C2B9                 db    ? ;
    .data:0040C2BA                 db    ? ;
    .data:0040C2BB                 db    ? ;
    .data:0040C2BC                 db    ? ;
    .data:0040C2BD                 db    ? ;
    .data:0040C2BE                 db    ? ;
    .data:0040C2BF                 db    ? ;
    .data:0040C2C0                 db    ? ;
    .data:0040C2C1                 db    ? ;
    .data:0040C2C2                 db    ? ;
    .data:0040C2C3                 db    ? ;
    .data:0040C2C4                 db    ? ;
    .data:0040C2C5                 db    ? ;
    .data:0040C2C6                 db    ? ;
    .data:0040C2C7                 db    ? ;
    .data:0040C2C8                 db    ? ;
    .data:0040C2C9                 db    ? ;
    .data:0040C2CA                 db    ? ;
    .data:0040C2CB                 db    ? ;
    .data:0040C2CC                 db    ? ;
    .data:0040C2CD                 db    ? ;
    .data:0040C2CE                 db    ? ;
    .data:0040C2CF                 db    ? ;
    .data:0040C2D0                 db    ? ;
    .data:0040C2D1                 db    ? ;
    .data:0040C2D2                 db    ? ;
    .data:0040C2D3                 db    ? ;
    .data:0040C2D4                 db    ? ;
    .data:0040C2D5                 db    ? ;
    .data:0040C2D6                 db    ? ;
    .data:0040C2D7                 db    ? ;
    .data:0040C2D8                 db    ? ;
    .data:0040C2D9                 db    ? ;
    .data:0040C2DA                 db    ? ;
    .data:0040C2DB                 db    ? ;
    .data:0040C2DC                 db    ? ;
    .data:0040C2DD                 db    ? ;
    .data:0040C2DE                 db    ? ;
    .data:0040C2DF                 db    ? ;
    .data:0040C2E0                 db    ? ;
    .data:0040C2E1                 db    ? ;
    .data:0040C2E2                 db    ? ;
    .data:0040C2E3                 db    ? ;
    .data:0040C2E4                 db    ? ;
    .data:0040C2E5                 db    ? ;
    .data:0040C2E6                 db    ? ;
    .data:0040C2E7                 db    ? ;
    .data:0040C2E8                 db    ? ;
    .data:0040C2E9                 db    ? ;
    .data:0040C2EA                 db    ? ;
    .data:0040C2EB                 db    ? ;
    .data:0040C2EC                 db    ? ;
    .data:0040C2ED                 db    ? ;
    .data:0040C2EE                 db    ? ;
    .data:0040C2EF                 db    ? ;
    .data:0040C2F0                 db    ? ;
    .data:0040C2F1                 db    ? ;
    .data:0040C2F2                 db    ? ;
    .data:0040C2F3                 db    ? ;
    .data:0040C2F4                 db    ? ;
    .data:0040C2F5                 db    ? ;
    .data:0040C2F6                 db    ? ;
    .data:0040C2F7                 db    ? ;
    .data:0040C2F8                 db    ? ;
    .data:0040C2F9                 db    ? ;
    .data:0040C2FA                 db    ? ;
    .data:0040C2FB                 db    ? ;
    .data:0040C2FC                 db    ? ;
    .data:0040C2FD                 db    ? ;
    .data:0040C2FE                 db    ? ;
    .data:0040C2FF                 db    ? ;
    .data:0040C300                 db    ? ;
    .data:0040C301                 db    ? ;
    .data:0040C302                 db    ? ;
    .data:0040C303                 db    ? ;
    .data:0040C304                 db    ? ;
    .data:0040C305                 db    ? ;
    .data:0040C306                 db    ? ;
    .data:0040C307                 db    ? ;
    .data:0040C308                 db    ? ;
    .data:0040C309                 db    ? ;
    .data:0040C30A                 db    ? ;
    .data:0040C30B                 db    ? ;
    .data:0040C30C                 db    ? ;
    .data:0040C30D                 db    ? ;
    .data:0040C30E                 db    ? ;
    .data:0040C30F                 db    ? ;
    .data:0040C310                 db    ? ;
    .data:0040C311                 db    ? ;
    .data:0040C312                 db    ? ;
    .data:0040C313                 db    ? ;
    .data:0040C314                 db    ? ;
    .data:0040C315                 db    ? ;
    .data:0040C316                 db    ? ;
    .data:0040C317                 db    ? ;
    .data:0040C318                 db    ? ;
    .data:0040C319                 db    ? ;
    .data:0040C31A                 db    ? ;
    .data:0040C31B                 db    ? ;
    .data:0040C31C                 db    ? ;
    .data:0040C31D                 db    ? ;
    .data:0040C31E                 db    ? ;
    .data:0040C31F                 db    ? ;
    .data:0040C320                 db    ? ;
    .data:0040C321                 db    ? ;
    .data:0040C322                 db    ? ;
    .data:0040C323                 db    ? ;
    .data:0040C324                 db    ? ;
    .data:0040C325                 db    ? ;
    .data:0040C326                 db    ? ;
    .data:0040C327                 db    ? ;
    .data:0040C328                 db    ? ;
    .data:0040C329                 db    ? ;
    .data:0040C32A                 db    ? ;
    .data:0040C32B                 db    ? ;
    .data:0040C32C                 db    ? ;
    .data:0040C32D                 db    ? ;
    .data:0040C32E                 db    ? ;
    .data:0040C32F                 db    ? ;
    .data:0040C330                 db    ? ;
    .data:0040C331                 db    ? ;
    .data:0040C332                 db    ? ;
    .data:0040C333                 db    ? ;
    .data:0040C334                 db    ? ;
    .data:0040C335                 db    ? ;
    .data:0040C336                 db    ? ;
    .data:0040C337                 db    ? ;
    .data:0040C338                 db    ? ;
    .data:0040C339                 db    ? ;
    .data:0040C33A                 db    ? ;
    .data:0040C33B                 db    ? ;
    .data:0040C33C                 db    ? ;
    .data:0040C33D                 db    ? ;
    .data:0040C33E                 db    ? ;
    .data:0040C33F                 db    ? ;
    .data:0040C340                 db    ? ;
    .data:0040C341                 db    ? ;
    .data:0040C342                 db    ? ;
    .data:0040C343                 db    ? ;
    .data:0040C344                 db    ? ;
    .data:0040C345                 db    ? ;
    .data:0040C346                 db    ? ;
    .data:0040C347                 db    ? ;
    .data:0040C348                 db    ? ;
    .data:0040C349                 db    ? ;
    .data:0040C34A                 db    ? ;
    .data:0040C34B                 db    ? ;
    .data:0040C34C                 db    ? ;
    .data:0040C34D                 db    ? ;
    .data:0040C34E                 db    ? ;
    .data:0040C34F                 db    ? ;
    .data:0040C350                 db    ? ;
    .data:0040C351                 db    ? ;
    .data:0040C352                 db    ? ;
    .data:0040C353                 db    ? ;
    .data:0040C354                 db    ? ;
    .data:0040C355                 db    ? ;
    .data:0040C356                 db    ? ;
    .data:0040C357                 db    ? ;
    .data:0040C358                 db    ? ;
    .data:0040C359                 db    ? ;
    .data:0040C35A                 db    ? ;
    .data:0040C35B                 db    ? ;
    .data:0040C35C                 db    ? ;
    .data:0040C35D                 db    ? ;
    .data:0040C35E                 db    ? ;
    .data:0040C35F                 db    ? ;
    .data:0040C360                 db    ? ;
    .data:0040C361                 db    ? ;
    .data:0040C362                 db    ? ;
    .data:0040C363                 db    ? ;
    .data:0040C364                 db    ? ;
    .data:0040C365                 db    ? ;
    .data:0040C366                 db    ? ;
    .data:0040C367                 db    ? ;
    .data:0040C368                 db    ? ;
    .data:0040C369                 db    ? ;
    .data:0040C36A                 db    ? ;
    .data:0040C36B                 db    ? ;
    .data:0040C36C                 db    ? ;
    .data:0040C36D                 db    ? ;
    .data:0040C36E                 db    ? ;
    .data:0040C36F                 db    ? ;
    .data:0040C370                 db    ? ;
    .data:0040C371                 db    ? ;
    .data:0040C372                 db    ? ;
    .data:0040C373                 db    ? ;
    .data:0040C374                 db    ? ;
    .data:0040C375                 db    ? ;
    .data:0040C376                 db    ? ;
    .data:0040C377                 db    ? ;
    .data:0040C378                 db    ? ;
    .data:0040C379                 db    ? ;
    .data:0040C37A                 db    ? ;
    .data:0040C37B                 db    ? ;
    .data:0040C37C                 db    ? ;
    .data:0040C37D                 db    ? ;
    .data:0040C37E                 db    ? ;
    .data:0040C37F                 db    ? ;
    .data:0040C380                 db    ? ;
    .data:0040C381                 db    ? ;
    .data:0040C382                 db    ? ;
    .data:0040C383                 db    ? ;
    .data:0040C384                 db    ? ;
    .data:0040C385                 db    ? ;
    .data:0040C386                 db    ? ;
    .data:0040C387                 db    ? ;
    .data:0040C388                 db    ? ;
    .data:0040C389                 db    ? ;
    .data:0040C38A                 db    ? ;
    .data:0040C38B                 db    ? ;
    .data:0040C38C                 db    ? ;
    .data:0040C38D                 db    ? ;
    .data:0040C38E                 db    ? ;
    .data:0040C38F                 db    ? ;
    .data:0040C390                 db    ? ;
    .data:0040C391                 db    ? ;
    .data:0040C392                 db    ? ;
    .data:0040C393                 db    ? ;
    .data:0040C394                 db    ? ;
    .data:0040C395                 db    ? ;
    .data:0040C396                 db    ? ;
    .data:0040C397                 db    ? ;
    .data:0040C398                 db    ? ;
    .data:0040C399                 db    ? ;
    .data:0040C39A                 db    ? ;
    .data:0040C39B                 db    ? ;
    .data:0040C39C                 db    ? ;
    .data:0040C39D                 db    ? ;
    .data:0040C39E                 db    ? ;
    .data:0040C39F                 db    ? ;
    .data:0040C3A0                 db    ? ;
    .data:0040C3A1                 db    ? ;
    .data:0040C3A2                 db    ? ;
    .data:0040C3A3                 db    ? ;
    .data:0040C3A4                 db    ? ;
    .data:0040C3A5                 db    ? ;
    .data:0040C3A6                 db    ? ;
    .data:0040C3A7                 db    ? ;
    .data:0040C3A8                 db    ? ;
    .data:0040C3A9                 db    ? ;
    .data:0040C3AA                 db    ? ;
    .data:0040C3AB                 db    ? ;
    .data:0040C3AC                 db    ? ;
    .data:0040C3AD                 db    ? ;
    .data:0040C3AE                 db    ? ;
    .data:0040C3AF                 db    ? ;
    .data:0040C3B0                 db    ? ;
    .data:0040C3B1                 db    ? ;
    .data:0040C3B2                 db    ? ;
    .data:0040C3B3                 db    ? ;
    .data:0040C3B4                 db    ? ;
    .data:0040C3B5                 db    ? ;
    .data:0040C3B6                 db    ? ;
    .data:0040C3B7                 db    ? ;
    .data:0040C3B8                 db    ? ;
    .data:0040C3B9                 db    ? ;
    .data:0040C3BA                 db    ? ;
    .data:0040C3BB                 db    ? ;
    .data:0040C3BC                 db    ? ;
    .data:0040C3BD                 db    ? ;
    .data:0040C3BE                 db    ? ;
    .data:0040C3BF                 db    ? ;
    
    .data:0040A608 unk_40A608      db 0A2h ; ó             ; DATA XREF: _main+74o
    .data:0040A609                 db  86h ; å
    .data:0040A60A                 db 0D5h ; +
    .data:0040A60B                 db  67h ; g
    .data:0040A60C                 db 0B1h ; ¦
    .data:0040A60D                 db  9Dh ; ¥
    .data:0040A60E                 db 0E8h ; F
    .data:0040A60F                 db  4Ch ; L
    .data:0040A610                 db  39h ; 9
    .data:0040A611                 db  22h ; "
    .data:0040A612                 db  33h ; 3
    .data:0040A613                 db  5Ah ; Z
    .data:0040A614                 db 0E1h ; ß
    .data:0040A615                 db  6Fh ; o
    .data:0040A616                 db  45h ; E
    .data:0040A617                 db  47h ; G
    .data:0040A618                 db  8Ch ; î
    .data:0040A619                 db    8
    .data:0040A61A                 db  6Bh ; k
    .data:0040A61B                 db  5Eh ; ^
    .data:0040A61C                 db  0Bh
    .data:0040A61D                 db  23h ; #
    .data:0040A61E                 db  30h ; 0
    .data:0040A61F                 db  49h ; I
    .data:0040A620                 db 0C4h ; -
    .data:0040A621                 db 0A0h ; á
    .data:0040A622                 db 0EEh ; e
    .data:0040A623                 db 0A6h ; ª
    .data:0040A624                 db    1
    .data:0040A625                 db 0F0h ; =
    .data:0040A626                 db  4Fh ; O
    .data:0040A627                 db 0EBh ; d
    .data:0040A628                 db  65h ; e
    .data:0040A629                 db  68h ; h
    .data:0040A62A                 db  40h ; @
    .data:0040A62B                 db 0C4h ; -
    .data:0040A62C                 db  4Eh ; N
    .data:0040A62D                 db    8
    .data:0040A62E                 db 0BAh ; ¦
    .data:0040A62F                 db  8Dh ; ì
    .data:0040A630                 db  7Ch ; |
    .data:0040A631                 db  46h ; F
    .data:0040A632                 db 0F3h ; =
    .data:0040A633                 db  96h ; û
    .data:0040A634                 db  3Eh ; >
    .data:0040A635                 db 0A2h ; ó
    .data:0040A636                 db  9Bh ; ¢
    .data:0040A637                 db  92h ; Æ
    .data:0040A638                 db  6Eh ; n
    .data:0040A639                 db 0E8h ; F
    .data:0040A63A                 db 0D0h ; -
    .data:0040A63B                 db  64h ; d
    .data:0040A63C                 db  2Ch ; ,
    .data:0040A63D                 db 0D0h ; -
    .data:0040A63E                 db 0C5h ; +
    .data:0040A63F                 db  18h
    .data:0040A640                 db  4Fh ; O
    .data:0040A641                 db  19h
    .data:0040A642                 db  33h ; 3
    .data:0040A643                 db  65h ; e
    .data:0040A644                 db  6Ch ; l
    .data:0040A645                 db  59h ; Y
    .data:0040A646                 db 0AEh ; «
    .data:0040A647                 db 0B3h ; ¦
    .data:0040A648                 db  4Bh ; K
    .data:0040A649                 db  44h ; D
    .data:0040A64A                 db  3Ch ; <
    .data:0040A64B                 db 0F2h ; =
    .data:0040A64C                 db 0DDh ; ¦
    .data:0040A64D                 db 0E5h ; s
    .data:0040A64E                 db  59h ; Y
    .data:0040A64F                 db    4
    .data:0040A650                 db 0CAh ; -
    .data:0040A651                 db  4Bh ; K
    .data:0040A652                 db  1Bh
    .data:0040A653                 db 0A2h ; ó
    .data:0040A654                 db  1Eh
    .data:0040A655                 db 0B7h ; +
    .data:0040A656                 db 0A6h ; ª
    .data:0040A657                 db  54h ; T
    .data:0040A658                 db  23h ; #
    .data:0040A659                 db    7
    .data:0040A65A                 db  15h
    .data:0040A65B                 db  11h
    .data:0040A65C                 db  74h ; t
    .data:0040A65D                 db 0A6h ; ª
    .data:0040A65E                 db  16h
    .data:0040A65F                 db  22h ; "
    .data:0040A660                 db  62h ; b
    .data:0040A661                 db 0C8h ; +
    .data:0040A662                 db  67h ; g
    .data:0040A663                 db  94h ; ö
    .data:0040A664                 db  48h ; H
    .data:0040A665                 db 0B3h ; ¦
    .data:0040A666                 db 0F2h ; =
    .data:0040A667                 db  1Fh
    .data:0040A668                 db 0C6h ; ¦
    .data:0040A669                 db  57h ; W
    .data:0040A66A                 db  30h ; 0
    .data:0040A66B                 db  66h ; f
    .data:0040A66C                 db 0A8h ; ¿
    .data:0040A66D                 db  7Ch ; |
    .data:0040A66E                 db  89h ; ë
    .data:0040A66F                 db    2
    .data:0040A670                 db  4Eh ; N
    .data:0040A671                 db 0CAh ; -
    .data:0040A672                 db 0F3h ; =
    .data:0040A673                 db  9Ch ; £
    .data:0040A674                 db  64h ; d
    .data:0040A675                 db 0F0h ; =
    .data:0040A676                 db 0F4h ; (
    .data:0040A677                 db  28h ; (
    .data:0040A678                 db  56h ; V
    .data:0040A679                 db 0A9h ; ¬
    .data:0040A67A                 db 0B4h ; ¦
    .data:0040A67B                 db 0EFh ; n
    .data:0040A67C                 db 0ACh ; ¼
    .data:0040A67D                 db 0E6h ; µ
    .data:0040A67E                 db  79h ; y
    .data:0040A67F                 db  84h ; ä
    .data:0040A680                 db 0CBh ; -
    .data:0040A681                 db  64h ; d
    .data:0040A682                 db  0Bh
    .data:0040A683                 db 0D3h ; +
    .data:0040A684                 db 0CEh ; +
    .data:0040A685                 db  6Fh ; o
    .data:0040A686                 db  6Ch ; l
    .data:0040A687                 db  60h ; `
    .data:0040A688                 db 0E5h ; s
    .data:0040A689                 db  14h
    .data:0040A68A                 db  62h ; b
    .data:0040A68B                 db  64h ; d
    .data:0040A68C                 db 0F8h ; °
    .data:0040A68D                 db  8Bh ; ï
    .data:0040A68E                 db  34h ; 4
    .data:0040A68F                 db  6Ch ; l
    .data:0040A690                 db 0F8h ; °
    .data:0040A691                 db  15h
    .data:0040A692                 db  33h ; 3
    .data:0040A693                 db  18h
    .data:0040A694                 db  14h
    .data:0040A695                 db  20h
    .data:0040A696                 db  4Eh ; N
    .data:0040A697                 db  20h
    .data:0040A698                 db 0CEh ; +
    .data:0040A699                 db  63h ; c
    .data:0040A69A                 db 0DCh ; _
    .data:0040A69B                 db  4Bh ; K
    .data:0040A69C                 db  22h ; "
    .data:0040A69D                 db  48h ; H
    .data:0040A69E                 db 0E7h ; t
    .data:0040A69F                 db  6Dh ; m
    .data:0040A6A0                 db  9Ch ; £
    .data:0040A6A1                 db 0D5h ; +
    .data:0040A6A2                 db  82h ; é
    .data:0040A6A3                 db  9Bh ; ¢
    .data:0040A6A4                 db  3Eh ; >
    .data:0040A6A5                 db 0F0h ; =
    .data:0040A6A6                 db  8Eh ; Ä
    .data:0040A6A7                 db 0BAh ; ¦
    .data:0040A6A8                 db 0FBh ; v
    .data:0040A6A9                 db  22h ; "
    .data:0040A6AA                 db  7Fh ; 
    .data:0040A6AB                 db    9
    .data:0040A6AC                 db  9Fh ; ƒ
    .data:0040A6AD                 db 0C2h ; -
    .data:0040A6AE                 db  67h ; g
    .data:0040A6AF                 db 0BBh ; +
    .data:0040A6B0                 db  7Dh ; }
    .data:0040A6B1                 db  2Dh ; -
    .data:0040A6B2                 db  6Ch ; l
    .data:0040A6B3                 db  75h ; u
    .data:0040A6B4                 db  2Dh ; -
    .data:0040A6B5                 db  61h ; a
    .data:0040A6B6                 db  77h ; w
    .data:0040A6B7                 db  0Bh
    .data:0040A6B8                 db 0C0h ; +
    .data:0040A6B9                 db  33h ; 3
    .data:0040A6BA                 db  2Ch ; ,
    .data:0040A6BB                 db 0EAh ; O
    .data:0040A6BC                 db  26h ; &
    .data:0040A6BD                 db  76h ; v
    .data:0040A6BE                 db    2
    .data:0040A6BF                 db  1Fh
    .data:0040A6C0                 db  2Bh ; +
    .data:0040A6C1                 db 0BBh ; +
    .data:0040A6C2                 db  93h ; ô
    .data:0040A6C3                 db 0B3h ; ¦
    .data:0040A6C4                 db  5Bh ; [
    .data:0040A6C5                 db  8Fh ; Å
    .data:0040A6C6                 db  72h ; r
    .data:0040A6C7                 db    7
    .data:0040A6C8                 db 0A1h ; í
    .data:0040A6C9                 db 0DAh ; +
    .data:0040A6CA                 db  99h ; Ö
    .data:0040A6CB                 db  41h ; A
    .data:0040A6CC                 db  70h ; p
    .data:0040A6CD                 db 0C7h ; ¦
    .data:0040A6CE                 db  52h ; R
    .data:0040A6CF                 db  7Dh ; }
    .data:0040A6D0                 db  55h ; U
    .data:0040A6D1                 db 0CBh ; -
    .data:0040A6D2                 db  19h
    .data:0040A6D3                 db  67h ; g
    .data:0040A6D4                 db 0B5h ; ¦
    .data:0040A6D5                 db  47h ; G
    .data:0040A6D6                 db  5Bh ; [
    .data:0040A6D7                 db  4Bh ; K
    .data:0040A6D8                 db  27h ; '
    .data:0040A6D9                 db 0D0h ; -
    .data:0040A6DA                 db  25h ; %
    .data:0040A6DB                 db 0E5h ; s
    .data:0040A6DC                 db  8Fh ; Å
    .data:0040A6DD                 db  90h ; É
    .data:0040A6DE                 db  8Bh ; ï
    .data:0040A6DF                 db 0F1h ; ±
    .data:0040A6E0                 db  93h ; ô
    .data:0040A6E1                 db  66h ; f
    .data:0040A6E2                 db  6Bh ; k
    .data:0040A6E3                 db 0BAh ; ¦
    .data:0040A6E4                 db 0E9h ; T
    .data:0040A6E5                 db  97h ; ù
    .data:0040A6E6                 db  52h ; R
    .data:0040A6E7                 db  31h ; 1
    .data:0040A6E8                 db 0AFh ; »
    .data:0040A6E9                 db 0CDh ; -
    .data:0040A6EA                 db  23h ; #
    .data:0040A6EB                 db  51h ; Q
    .data:0040A6EC                 db 0C1h ; -
    .data:0040A6ED                 db 0B3h ; ¦
    .data:0040A6EE                 db  4Bh ; K
    .data:0040A6EF                 db  54h ; T
    .data:0040A6F0                 db 0BBh ; +
    .data:0040A6F1                 db 0DBh ; ¦
    .data:0040A6F2                 db  96h ; û
    .data:0040A6F3                 db 0F7h ; ˜
    .data:0040A6F4                 db 0B6h ; ¦
    .data:0040A6F5                 db  59h ; Y
    .data:0040A6F6                 db    7
    .data:0040A6F7                 db  57h ; W
    .data:0040A6F8                 db  3Dh ; =
    .data:0040A6F9                 db  21h ; !
    .data:0040A6FA                 db  2Eh ; .
    .data:0040A6FB                 db 0A8h ; ¿
    .data:0040A6FC                 db 0B7h ; +
    .data:0040A6FD                 db 0A8h ; ¿
    .data:0040A6FE                 db  69h ; i
    .data:0040A6FF                 db 0D0h ; -
    .data:0040A700                 db 0B0h ; ¦
    .data:0040A701                 db  5Bh ; [
    .data:0040A702                 db  17h
    .data:0040A703                 db 0A1h ; í
    .data:0040A704                 db 0B7h ; +
    .data:0040A705                 db 0C8h ; +
    .data:0040A706                 db  8Eh ; Ä
    .data:0040A707                 db    0
    .data:0040A708                 db    0
    .data:0040A709                 db    0
    .data:0040A70A                 db    0
    .data:0040A70B                 db    0
    .data:0040A70C                 db    0
    .data:0040A70D                 db    0
    .data:0040A70E                 db    0
    .data:0040A70F                 db    0