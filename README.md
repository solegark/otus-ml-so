# otus-ml-so
Учебный проект OTUS-ML.

# Антфрод система

## Постановка:

Бюджет - 10М рублей
Срок реализации: 
  - 3 месяца (MVP),
  - 6 месяцев - готовый проект


Статистика: 
 - 2 транзакции на 100 - реальные мошеннические схемы (точность 98%)
 - Общий ущерб клиентов не больше 500 000 рублей

Нагрузка:
50 транзакций в секунду, пик - 400 транзакций

Ограничение:
Более 5% FP - отток клиентов

Эксплуатация:
Сервис на внешних мощностях (облачное решение?)


Датасеты - 
csv-файлы с транзакциями

Инфобез: 
Конфиденциальная информация - утечка недопустима


Mission CANVAS

<!--[if IE]><meta http-equiv="X-UA-Compatible" content="IE=5,IE=9" ><![endif]-->
<!DOCTYPE html>
<html>
<head>
<title>MBM.html</title>
<meta charset="utf-8"/>
</head>
<body>
<div class="mxgraph" style="max-width:100%;border:1px solid transparent;" data-mxgraph="{&quot;highlight&quot;:&quot;#0000ff&quot;,&quot;nav&quot;:true,&quot;resize&quot;:true,&quot;xml&quot;:&quot;&lt;mxfile host=\&quot;Electron\&quot; modified=\&quot;2024-01-15T09:31:54.817Z\&quot; agent=\&quot;5.0 (Windows NT 10.0; Win64; x64) AppleWebKit/537.36 (KHTML, like Gecko) draw.io/19.0.1 Chrome/100.0.4896.160 Electron/18.3.2 Safari/537.36\&quot; etag=\&quot;CcaAJNrCt2cR-LtPi_8b\&quot; version=\&quot;19.0.1\&quot; type=\&quot;device\&quot;&gt;&lt;diagram id=\&quot;07fea595-8f29-1299-0266-81d95cde20df\&quot; name=\&quot;Page-1\&quot;&gt;7Vxbb6u4Fv41eUzEnfCYpGSPdGakrd3RzOMWJU6CSiAHnLZ7fv3YYMwyNikQknSk9IESY2Ovy7duBibm6vDxLQuO+z/SDYonhrb5mJhPE8OwbdMk/2jLr7JFdwzWssuiDWurG56jfxBr1FjrKdqgXOiI0zTG0VFsDNMkQSEW2oIsS9/Fbts0Fmc9BjskNTyHQSy3/h1t8J616o5XX/gNRbs9m3puuOWFlyB83WXpKWHzJWmCyiuHoLoNozHfB5v0HTSZ/sRcZWmKy7PDxwrFlK8Vx8px65arfMkZSnCXAY43L4e8BfGJ0c1Whn9VjChIQXSENjGX7/sIo+djENKr70T2pG2PDzH5pZNTThHtGwcvKF5ydqzSOM3IpYIhpCvO0lekbKwYbpKWbRTHVaeJYaI52mzpzbdpgpnWONVv0M9Y20t3RdqDONolpC1GW8KTpcwixrU3lGH0AZoYy76h9IBw9ot0YVenhuExATLlttjP91pRCAZY4x4qyZw1Bkw7d/zutZjICZNUm9Q8hdScmJK3id4E6Tn/P1FlKrgzzQt2LUgHwzl+1BfJ2Y79j6vOw++yOuWYEJWRDj9QHOAoTfI9RS27OyGvnECclDQXixdbFU0vWe+hU7KWCVHJhU6Py/mE6OpcL45G0WIXx1Vx1Fjn5broUJ77xRF2tsD5E7jtuhrug0tLdmd69Fh7PQvs0FiSA869NnrvAliIRRG1tozabfEnolY3uqOWgjMitnnBmnFKycgJVVGyo4ZCGwnani0im5tqAG3LUCDb0EZAtlvdRIFsFWYuA+r/EKX8e5DhBGWfwVOJukvWpBvnTBCdbug9KrR7HO3k6AI02iX+pwCUT+B8CdBsgFss2DkDrguGLMC5Wwx0pYHUrkxVtgXaE18yTRqwPEuVzSla2G0tyYxo1Q053QZfDRiyVNmuchkmoEdp7lZgFGlxpJ4LccYFWJgLFgaphovkjNKqVfG5jOK4rLpBMiHf5uCqVnc2IKN8sB5Z0g1hKQ3+J+pWzd7EE3dOkEi3A9myio2jm/Nq7Q1fZIpr4qKGbBgsBOiZZZ/sVw5wMHkqrn+L8G+nF056qesNcEIK/G4glOMGu1pLA9WrSmorERu+aBEAHhQKJ7Kkr7nuGDBez1o/gpqrBzV1Ut03qrHHiWr0m0c1ixBHbxGOUJe4ZgTVbadj/OkUiY13JoopjENtZblH99pdL+/jg56lbR4QalQWrHe21sshCr7sj7++V+uEDgTmbBV/hG4lCXPRDfKjX7nB4nxIqOQEB4rx5CU/DslfPResEkrFUFG+lhxxFWkOdKM+49TwZXeYyICqzLWtYrpCq+QI0RV9diNogdNBxS31ftU1jBHWqYmj4AobsFmBVXngDo3Av1CXauBUmLieBkYiymBBGaGU9BRhc92hEaJzpdbE0gQPa8vhnDCoYRxAcojUWsG4hg04Zulm2m1pDJyXLa2vyimE03/JF9qTu4f6bUW4sQJ+NSskh/0INkcLNnXXG1pCs0cJNo3zxfHxY80fKE9PWfhpqHnNCndhkOQSAcxqLcnkVEUDSuGwSjoMMRxwZ7mQBj3bUoxQ/EnvGGzF6Oodg/n9baSczjesI1/5qp3evpNeq3T5FcQMheoDNbUkJYBzwe0UqArcR3BnxFnmg9mh61FGXL34cwlSLwO5ZwHOc27waM4eAmavWy43WsG4Y2L2lWTxCBCuFyBY7m0DBPMr757/VazK0L5n6THNo2L3/J5xBWsiepB0qlxphKhiWNum3PmdL1iCgumHp7ImGkhpbWBilJ2h6ZH37uFuuzK91VXLlipnQobji2PhVpdcwuBOeilQV6/nzBAeE0Fv12AUtKelML+UJii3DqHX8aWoUAe0t5WNDCDKhsJA/8SLPqaKsbxCwn2b9pl0erH64VvG8y2me9+dDut2ySd4zuoZ7Q6Ea1/BUVzwdJb3qQGEScUA03fJk2Mwk14IYBeiWMkj1I5gsLl+GIvrGAvbvK+tsG9oK/ZBkqD43hUqdb25UQCoHnbsVzOGpuGTJy+nAHkdn7scDb5nCnfeip03gsj6qHeLbrvEkVUK/rAyt36i1NKtblbG1JwxrIzzlbPdVZrT0c84O4X4lKE726cFhP2S7wdPVZBcSDkq3PuCm8ka2L+ClflGy1LqrI2y2TWi+YalZjkJg9vRjcdE4Jao+BRFbWAbu56wllhvIDZE0b8wfdvHPXqo3jm1mIqzt7kuvn0P3awl3VcX1RCGtbwd8v2RuN7hET1XEYzqmuqdIt0ZJRp1v7Kf+IHeUFLURYmrQMHhK7xM5OmitToDzCfRhih3UG5W/XtA+DoQ1jkQ7wVh+WXOP/cUM8tTHiUoJ6DRqhd1V0HyFuQqFDQ0glCPRbFniKA1eCk6UN4d04iWnkhvezmxn6gETjjNmaR6CuRP+uNpaonyPvuC51XMr67LsnPnCtG5o0hO9UJnQxBAAhUHf6eY+852ici1lxTj9NAORoimFilASG+CfM9tgYhTq+x7pGs7fOzoK+CzKM3d2SHKw1m4R+GrCvVcZm0YJ3faRKiWMzMfA6E/Cqqt5rPztiFphip908fI3qq5zylGUw454UE+w1nwhuLZkaC1oB4iuMF9zj7lG9mfKptakypRhGR2lPXzFl3FPYp8Na0hX9OW5GvqsnytMYCvq96MuAvwpffulcrQqjntdkNlJaIwJSq6R0GG74tu27NmHvhzRVWwZKhbClUwR4G6qhwsQ72FzTAsUwkubmgMh+VAeDfFesjDAM3COD1tZpsABz+3QYhTwoJ2neluA278eQfdsholO08OBlRh3CiPp+iqgl1Xk5/kxzTDxTcXZrSm9vrT+e+a/rNiz4/lR1+20QcFwVjWQJS7JbsC62pyVyXgLXKPDsXHa5YK1yCKYgyHUUy2qPitqZjP1vO0x5h+nWdBqTbW4SaxClO/jUhSmc1CMiNJP4l1IP8KF0D+o7conhY/pqccZdOI6syWppzG2iHiWB+zKERT3ZjPjjRfE5Wpa16p+JAMV6UOMeetDZDRzCQVMac9VyjifAxF7PBNoFbf0zBMwXtululAHOX4Z0jL/b0lcYVvCt1PtjxXOCNax53ZsnBdewzhdsg0h0cZZ139iNFHesJxlJDZq09/qSLNdLslloNYnSRER5zPyIjXS/2PVvxdCfVzV2+En7qsGorwk3/17BLFMDpkmpRjx+6k8m+zsWLRBH7kTA0Ozaw0n/NAdsHVF9hGd8FGh2xsADiI3qyLvzsjgfrXvDheKypvg4dogQ0lYGoN7AwZU8TLVBGtOddSFeOhKv8JVRlfGcjP+guNxTXwCUzT/xc=&lt;/diagram&gt;&lt;/mxfile&gt;&quot;,&quot;toolbar&quot;:&quot;pages zoom layers lightbox&quot;,&quot;page&quot;:0}"></div>
<script type="text/javascript" src="https://app.diagrams.net/js/viewer-static.min.js"></script>
</body>
</html>
