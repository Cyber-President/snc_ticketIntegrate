# snc_ticketIntegrate
Consolidate tickets to the same destination / 同一送付先のチケットを統合する


### Import CSV file sample.
| no | ticket_no | name_jp | name_alp | e-mail | token | ticket_url |
| ---- | ---- | ---- | ---- | ---- | ---- | ---- |
| 1 | AAAA-BBBB-CCCCC | わかめゆでたろう | wakameyudetaro | info@sample.com | https://www.wixevents.com/check-in/AAAA-BBBB-CCCCC,zzzzzzzz-12345678 | https://drive.google.com/file/d/***sample1***/view?usp=drivesdk |
| 1 | DDDD-EEEE-FFFFF | わかめゆでたろう | wakameyudetaro | info@sample.com | https://www.wixevents.com/check-in/DDDD-EEEE-FFFFF,yyyyyyyy-23456789 | https://drive.google.com/file/d/***sample2***/view?usp=drivesdk |

### Export CSV file sample.
|  | 0 | 1 | 2 | 3 | 4 | ... |
| ---- | ---- | ---- | ---- | ---- | ---- | ---- |
| 0 | info@sample.com | AAAA-BBBB-CCCCC | https://drive.google.com/file/d/***sample1***/view?usp=drivesdk | DDDD-EEEE-FFFFF | https://drive.google.com/file/d/***sample2***/view?usp=drivesdk |  |