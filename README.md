# API Gateway

API Gateway, istemcilerle backend sunucuları / mikro servisler arasında duran bir API yönetim aracıdır.

API Gateway, API isteklerini alarak çeşitli kurallara göre uygun servislere yönlendiren bir ``` reverse proxy``` olarak çalışır. API Gateway istek sınırlandırma, istatistik, kimlik doğrulama vs. çeşitli sık kullanılan işlevleri üzerine alarak asıl API sunucularınızın önünde bir üst katman oluşturur.

Son yıllarda kullanılan API’ların yönetiminden doğan zorluklara karşı Amazon Web Service tarafından getirilen bir çözümdür.

![photo](https://www.gencayyildiz.com/blog/wp-content/uploads/2020/06/Microservice-Mimarisinde-API-Gateway-Nedir.png)


###  API Gateway İle Neler Yapılabilir?

#### Authentication ve Authorization

İşlevsel sorumluluğu parça parça üstlenen servislere erişim api gateway üzerinden dolaylı yolla olacağından dolayı kimlik ve yetki doğrulama operasyonlarını sadece api gateway’de yapılandırılabilir.

#### Logging

Servislere yapılan istekler hakkında detaylı loglamalar gerçekleştirilebilir ve böylece hangi servis, kim tarafından, ne kadar yoğunlukta işlevsellik gösteriyor vs. gibi istatistiksel bilgiler edinilebilir.

#### Response Caching

API gateway üzerinden servislere gelen talepler neticesinde üretilen çıktıları cacheleyebilir ve böylece servis maliyetleri düşürülebilir.

#### Routing

Servislerin adreslerini farklı şekilde kapsüllenebilir ve bu kapsül üzerinden clientlar ilgili esas routelara yönlendirilebilir.
Yukarıdaki maddelere baktığımızda API Gateway ile yazılımda problemlerin ve işlevsel operasyonların yapıldığı esas kod merkezlerinin dışında kalan ve problem alanından bağımsız kısımları ilgilendiren cross cutting concern ismi verilen alanları ve işlemleri yönetebildiğimizi görebilmekteyiz.




