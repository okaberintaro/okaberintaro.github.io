---
layout: post
title:  "Anonimliğe Yaklaşmak"
date:   2021-06-17 18:32:06 +0000
categories: blog
---

Evet arkadaşlar. Anonim bir blog kurdum dedim, blogun ilk yazısı olarak da nasıl anonim kalınacağını, nasıl anonimliğe yaklaşılacağını anlatalım öyleyse.

Öncelikle şunu belirtmek isterim ki, internet ortamında %100 anonimlik diye bir şey yoktur. En fazla bu oranı yükseltebilirsiniz. Yani siz bir şekilde internete bağlanıyorsanız, bir yerlerde anonimliği bozacak bir etken mutlaka vardır.
Bugünki anonimlik yazıları ve eforları hiç bir zaman %100 anonimlik sağlamak üzerine kurulmamıştır zaten.

Pekyleyse, bu anonim olduğunu iddia eden sistemler nasıl çalışıyor?
Şöyle çalışıyor, sizi tam olarak anonim etmek yerine takibi çok zor bir hale getiriyorlar. Yani bir şeyi ne kadar zor takip edersen o kadar anonim kalırsın aslında. Örneğin TOR'dan bahsedelim. İnternette dolaşırken kimliğimizi gizlemek istiyorsak TOR güzel bir imkan tanıyor bizlere.
asdasd
TOR Nasıl Çalışıyor?
Cevabı çok basit değil aslında ancak şöyle de açıklanabilir, bir takım bilgisayarların birleşiminden oluşmuş, alternatif bir internet teknolojisi diyebiliriz. Yani, "onion network" deniyor buna. Tabii gene internet altyapısı için döşenmiş olan fiberoptik kabloları kullanıyorsunuz bu sisteme de erişmek için ancak yapısı biraz daha farklı şekilde çalışıyor.
Siz TOR'a bağlandığınız zaman öncelikle TOR ağında bunu işletecek bir node'a bağlanmanız gerekmekte. Daha sonrasından o node da başka nodelara bağlanarak bir kanal oluşturuyor ve giriş-çıkış IP'leri arasında birden çok fark oluşmuş oluyor.


Yani şöyle çalışıyor aslında node sistemi (ülkeleri örnek verdim):

Sizin internetiniz -> Node 1 (Fransa)
Node 1 (Fransa) -> Node 2 (Almanya)
Node 2 (Almanya) -> Node 3 (Belarus)
...
Node 5 (Macaristan) -> Node 6 (Japonya)

Yani bulunduğunuz ülkeden bir giriyorsunuz, Japonya'dan çıkıyorsunuz. Japonya'dan çıkana kadar da farklı ülkelerde bulunan makinelerden gir-çık yaparak direkt olarak takip edilmesi çok zor olan bir hale getiriyorsunuz.
Ancak ve ancak! Buraya dikkat. Eğer bu örneğimizde Fransa'da bulunan Node 1'deki kişi loglamayı açtıysa, işte sizi takip etmek isteyen birisinin eline düşerse eğer bu Node 1, o zaman anonimlik falan yalan olur. Yani gene takip edilmesi zor ama sizi takip etmek için elinde TOR Node'u bulundurabilecek kapasitede birisi, burdaki loglarınızla geriye dönük takip yapma yeteneğine de muhtemelen sahiptir.

Bu yüzden de gene dikkatli olmakta fayda var. Tabii buna karşı ne yapabilirsiniz? Zaten Whonix sitesinde de dediği gibi, eğer maksimum anonim olmak istiyorsanız, bu alemde, asla ama asla kendiniz olmayacaksınız.
Kendinizle alakalı bağlantısı bulunan en ufak bir hesabı bile kullanmayacaksınız. Whonix'i açmadan önce, TOR network'e çıkmadan önce bile VPN kullanacaksınız. Bu bağlantı hızınızı olumsuz yönde etkilese de zaten anonim bir şekilde oturup da 4k video izlemeyeceksiniz herhalde.

Aşağıda maddeleri sıralayalım:
1- Whonix imajını şifreli bir şekilde, gene şifreli olan bir disk içerisinde saklayın.
2- Parolalarınız için Whonix içinde bulunan Keepas'i kullanın ve kesinlikle bu parolaları host bilgisayara (yani Virtualbox'un kurulu olduğu bilgisayara) çıkartmayın.
3- DNS-Over-TLS kullanın. DNS-Over-HTTPS de iş görür ama "it's an ugly hack" yani çirkin. DOT kullanın yani.
4- Whonix'e bağlanmadan önce bir VPN üzerinden bağlanın mutlaka. Eğer mümkünse İsviçre tabanlı bir sanal makine sağlayıcısı, host sağlayıcısı bir yerlerden server alıp sonrasında OpenVPN setup'ıyla giriş yapın. OpenVPN ayarlamalarını da obfsproxy kullanacak şekilde yapın.
5- Whonix'i kesinlikle kendiniz olarak kullanmayın. Bir persona oluşturun kendinize ve her zaman o şekilde kullanın.
6- Hava basmak için sağa sola bunu anlatmayın. Kendinizi hedef haline getirmeyin.
7- Tarayıcınızda Javascript'leri açmayın.
8- Whonix üzerinde kullandığınız hesaplarınıza, kendi Whonix imajınız hariç bir yerden erişmeyin.
9- Tarayıcınızı tam ekran yapmayın. Her zaman açıldığı ekranda gezin.
10- Host saatiniz ile guest saatiniz de farklı olsun.
11- Ne olduğunu biliyorsanız I2P kullanın.
12- Bilmediğiniz şeyleri bilgisayarınızda çalıştırmayın.

Tavsiyelerim bu kadar. Elbette unuttuklarım da vardır. Her gün bizi takip eden ve her hareketimizi dava etmeye hazır bekleyen hükümetin radarından bu şekilde sıyrılabilir, istediğiniz her türlü şeyi bu şekilde yapabilirsiniz. Hadi bakalım geçmiş olsun.

İlerleyen dönemlerde "TOR üzerinde web sitesi kurmak ve işletmek" kısmını şöyle özet halinde sizlere anlatacağım
