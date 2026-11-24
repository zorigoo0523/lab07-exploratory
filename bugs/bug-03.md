# BUG-03: Буруу JSON биетэй POST хүсэлтэд 400 статус код буцаахгүй байх

Орчин:  Уншлагын жагсаалт v2.0, curl, Ubuntu Linux, 2026-11-24
Урьдчилсан нөхцөл: node app.js-ийг шинээр асаасан (анхны 3 ном)

## Дахин гаргах алхам
1. Терминалд node app.js командыг ажиллуулна.
2. Шинэ терминал дээр curl -i -X POST http://localhost:3000/api/books -H "Content-Type: application/json" -d 'invalid-json' командыг ажиллуулна.

Хүлээгдэж байсан: Буруу JSON биетэй POST хүсэлтэд 400 алдаа буцаана.
Бодит үр дүн:     evidence/bug-03-curl.txt файлд гарсан HTTP статусыг энд бичнэ.

Ноцтой байдал: Major — API-ийн оролтын шалгалтын зөрчил.
Хавсралт:      evidence/bug-03-curl.txt
Олдсон аялал:  Saboteur
