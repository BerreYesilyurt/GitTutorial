## Git Nedir?
Git, versiyon kontrol sistemidir. Projemizde versiyonlar arası geçiş yapmamızı sağlar. Projenin yedeğini almak ya da güncellemeleri profesyonel olarak kaydedtmek için kullanabiliriz.

İlk olarak Git'i kullanabilmemiz için bilgisayarımızda kurulu olması gerekmektedir. Git kurulumunu [buradan](https://git-scm.com/downloads) yapabilirsiniz.

Git kurulumunu gerçekleştirdikten sonra bilgisayarımıza üç adet araç inmektedir.
- Git Bash
- Git Cmd
- Git GPU

Git Bash ve Git Cmd, git özelliklerini komut satırı ile kullanmamızı sağlar. Eğer Windows işletim sisteminde terminal kullanmaya alışıksanız Git Cmd, Linux işletim sisteminde terminal kullanmaya alışıksanız Git Bash kullanmanız önerilir.

Git GPU ise terminal kullanmakta zorlanan ya da terminal kullanmayı tercih etmeyen kullanıcılara yönelik hazırlanmış bir Grafik Kullanıcı Arayüzü'dür.

Ben bu yazıda Git Bash ile kullanabileceğimiz komutlardan bahsettim.

---
## Git Kullanımı
Genel ayarlardan bahsedecek olursak :
1- `git --version ` ile bilgisayarınızda yüklü olan git sürümünü öğrenebilirsiniz.  
  
2- `git config --list` ile git'in ilgili yapılandırılmış ayarlarını görebilirsiniz.  

3- `git config --global user.name "kullanmak istediğiniz kullanıcı adınız"` ve `git config --global user.email "mail adresiniz"` ile Git kullanıcı adınız ve mailinizi belirleyebilirsiniz.  

4- `cd` komutu ile bilgisayarda bulunan istediğiniz dizine gidebilirsiniz. Örneğin `cd/Desktop/GitTutorial` komutu ile masaüstünde bulunan GitTutorial klasörünün içine girmiş oluruz.  

5- `ls` komutu ile içerisinde bulunduğumuz klasörün içerdiği dosya ve dizinlere ulaşabiliriz. `ls -a` komutu ile gizli dosyaları da görmek mümkündür.  

6- `pwd` komutu ile hangi dizinde bulunduğumuzu soegulayabiliriz.

İlk olarak terminalde projemizin olduğu dizine gitmeliyiz. Bunun için "cd" komutunu kullanıyoruz. Örneğin terminalde `cd/Desktop/GitTutorial` komutu ile masaüstünde bulunan GitTutorial klasörüne girmiş oluruz.

` git init ` komutu ile projemizin bulunduğu klasöre ".git" uzantılı gizli bir klasör eklenir ve projemizde yaptığımız değişiklikler izlenir. Git komutlarını projemizde kullanabilmemiz için bu komutu kullanmamız şarttır. 




