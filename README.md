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