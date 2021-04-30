# snc_ticketIntegrate
Consolidate tickets to the same destination / 同一送付先のチケットを統合する


### Import CSV file sample.
| no | ticket_no | name_jp | name_alp | e-mail | token | ticket_url |
| ---- | ---- | ---- | ---- | ---- | ---- | ---- |
| 1 | AAAA-BBBB-CCCCC | わかめゆでたろう | wakameyudetaro | happy@wakame.com | https://www.wixevents.com/check-in/AAAA-BBBB-CCCCC,zzzzzzzz-12345678 | https://drive.google.com/file/d/***sample1***/view?usp=drivesdk |
| 2 | DDDD-EEEE-FFFFF | わかめゆでたろう | wakameyudetaro | happy@wakame.com | https://www.wixevents.com/check-in/DDDD-EEEE-FFFFF,yyyyyyyy-23456789 | https://drive.google.com/file/d/***sample2***/view?usp=drivesdk |
| 3 | GGGG-HHHH-IIIII | こんぶほしこ | konbuhoshiko | unhappy@konbu.com | https://www.wixevents.com/check-in/GGGG-HHHH-IIIII,xxxxxxxx-34567890 | https://drive.google.com/file/d/***sample3***/view?usp=drivesdk |


### Export CSV file sample.
|  | 0 | 1 | 2 | 3 | 4 | ... |
| ---- | ---- | ---- | ---- | ---- | ---- | ---- |
| 0 | happy@wakame.com | AAAA-BBBB-CCCCC | https://drive.google.com/file/d/***sample1***/view?usp=drivesdk | DDDD-EEEE-FFFFF | https://drive.google.com/file/d/***sample2***/view?usp=drivesdk |  |
| 1 | unhappy@konbu.com | GGGG-HHHH-IIIII | https://drive.google.com/file/d/***sample3***/view?usp=drivesdk |  |  |  |


### References
 - [pandasでcsvファイルの書き出し・追記（to_csv）](https://note.nkmk.me/python-pandas-to-csv/)
 - [pandasで欠損値NaNを前後の値から補間するinterpolate](https://note.nkmk.me/python-pandas-interpolate/)
 - [（Gスプレッドシート）改行をはさんで文字列を結合する](https://www.officeisyours.com/entry/2020/03/29/124906)
