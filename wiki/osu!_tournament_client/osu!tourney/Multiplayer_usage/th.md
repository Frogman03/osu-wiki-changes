# การใช้งานในห้องผู้เล่นหลายคนของ osu!tourney

## การสร้างห้อง

ห้องผู้เล่นหลายคนนั้นต้องตั้งชื่อโดยอ้างอิงจากรูปแบบที่แสดงขึ้นในแผงควบคุมของ osu!tourney

รูปแบบจะประกอบไปด้วย: 
`Acronym_in_tournament.cfg: (ชื่อทีม 1) vs (ชื่อทีม 2)`

`Acronym_in_tournament.cfg` จะถูกแทนที่ด้วยค่าของ `acronym` ในไฟล์ `tournament.cfg` จาก [การติดตั้ง](/wiki/osu!tourney/Setup).
ถ้าค่าถูกตั้งเป็น `Test Tourney` ตัวรูปแบบก็จะออกมาเป็น `Test Tourney: (ชื่อทีม 1) vs (ชื่อทีม 2)`.

ซึ่งชื่อทีม (`ชื่อทีม 1` and `ชื่อทีม 2`) สามารถโดนแทนที่ด้วยชื่อทีมอะไรก็ได้ **แต่อย่าเอาวงเล็บ `()` ที่ล้อมไว้ออก**

## การจัดการห้อง

### คำสั่งการจัดการทัวร์นาเมนต์

*หน้าหลัก: [คำสั่งการจัดการทัวร์นาเมนต์](/wiki/osu!tourney/Tournament_management_commands)*

อย่าลืมให้ช่องที่ถูกต้องกับผู้เล่นที่เข้าห้องมาแล้วโดยการใช้คำสั่ง `!mp move` และ `!mp team`

อย่างที่อธิบายไปใน [การใช้งานในการรับชม](/wiki/osu!tourney/Spectator_usage) แต่ละหน้าต่างของ client จะแสดงถึงช่องแต่ละอันในห้องผู้เล่นหลายคน หลังจากที่ตั้งค่า `TeamSize` ในไฟล์ `tournament.cfg` ทีมสีน้ำเงินจะใช้ `TeamSize` ช่องแรก และทีมสีแดงจะใช้ `TeamSize` ช่องข้างล่างสีน้ำเงิน

ตัวอย่าง: ถ้า `TeamSize = 4` ช่องที่ 1, 2, 3, 4 จะเป็นของทีมสีน้ำเงิน และช่องที่ 5, 6, 7, 8 จะเป็นของทีมสีแดง ถ้า `TeamSize = 3` ช่องที่ 1, 2, 3 จะเป็นของสีน้ำเงิน และช่องที่ 4, 5, 6 จะเป็นของทีมสีแดง

![หน้าต่างแต่ละอันใน osu!tourney ที่จะแสดงถึงเลขช่องแต่ละอันในห้องผู้เล่นหลายคน](img/Osutourneyassignment.png "การจัดวางผู้เล่นของ osu!tourney")

**osu!tourney ไม่สนใจสีของทีมในการจัดช่อง** - มันสนใจเพียงแค่ตำแหน่งของช่องที่ผู้เล่นอยู่เท่านั้น ด้านล่างจะเป็นตัวอย่างของ osu!tourney ในขนาดทีมต่าง ๆ เลขบนหน้าจอแสดงถึงเลขของช่องที่ผู้เล่นอยู่ในห้องผู้เล่นหลายคน ตัวเลขนั้นจะไม่แสดงขึ้นตอนใช้จริงและ มีไว้เพื่อกรณีศึกษาเท่านั้น :

![TeamSize = 4](img/Osutourneywindows.png)

![TeamSize = 3](img/Teamsize3.png "TeamSize = 3")

![TeamSize = 2](img/Teamsize2.png "TeamSize = 2")

![TeamSize = 1](img/Teamsize1.png "TeamSize = 1")
