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
## Git Bash İçin Temel Komutlar

1- `cd` komutu ile bilgisayarda bulunan istediğiniz dizine gidebilirsiniz. Örneğin `cd/Desktop/GitTutorial` komutu ile masaüstünde bulunan GitTutorial klasörünün içine girmiş oluruz.  

2- `ls` komutu ile içerisinde bulunduğumuz klasörün içerdiği dosya ve dizinlere ulaşabiliriz. `ls -a` komutu ile gizli dosyaları da görmek mümkündür.  

3- `pwd` komutu ile hangi dizinde bulunduğumuzu soegulayabiliriz.  

4- `mkdir "oluşturmak istediğiniz klasör adı"` yazarak termianl aracılığıyla bir klasör oluşturabiliyoruz.  

5- `touch "dosya adı"` ile bir dosya oluşturabiliyoruz. 

6- `vi ""dosya adı"` ile yazdığınız dosyanın içerisine girerek değişiklik yapabiliyorsunuz. Ancak bu komutu yazdıktan sonra değişiklik yapabilmeniz için **"i"** tuşuna basmanız gerekmektedir. Değişiklikleri tamamladıktan sonra dosyadan çıkabilmek için **"Esc"** tuşuna bastıkdan sonra **":wq"** yazmalısınız. Buradaki w-> write, q-> quit anlamına gelmektedir.  

7- `clear` komutu ile terminal ekranımızı temizleyebiliyoruz.

---
## Temel Git Komutları


1- `git --version ` ile bilgisayarınızda yüklü olan git sürümünü öğrenebilirsiniz.  
  
2- `git config --list` ile git'in ilgili yapılandırılmış ayarlarını görebilirsiniz.  

3- `git config --global user.name "kullanmak istediğiniz kullanıcı adınız"` ve `git config --global user.email "mail adresiniz"` ile Git kullanıcı adınız ve mailinizi belirleyebilirsiniz.  

4- Terminalde projemizin olduğu dizine gittikten sonra ` git init ` komutu ile projemizin bulunduğu klasöre ".git" uzantılı gizli bir klasör eklenir ve projemizde yaptığımız değişiklikler izlenir. Git komutlarını projemizde kullanabilmemiz için bu komutu kullanmamız şarttır.  

5- `git status` komutu projemizde bulunan dosyaları, durumlarını, staging area içerisinde bulunup bulunmadıklarını ve commit edilip edilemeyeceklerini gösterir.  

6- `git add "dosya adı"` ile istediğimiz dosyayı staging area'ya ekleyebiliyoruz. Eğer klasörümüzde bulunan tüm dosyaarı eklemek istersek bunun için kullanılması gereken kod ise şudur : `git add .` 

7- `git rm -cached "dosya adı"` komutu ile, stagng area'ya taşıdığımız dosyaları geri alabiliriz.

8- Dosyaları staging area'ya taşıdıktan sonra artık commit işlemi yapabiliriz. Commit, proje üzerinde yapılan her bir değişikliğin mesajla adlandırılması olarak tanımlanabilir. Yaptığımız değişikliği adlandırmak için `git commit -m "mesaj ifadesi"` komutunu kulanırız.

9 `git log` komutu ile yaptığımız commit işlemlerinin özet bilgilerini görüntüleyebiliriz. Eğer özet bilgilerinin daha okunabilir bir formatta gelmesi isteniyorsa `git log --oneline` komutu kullanılabilir.

10- `git branck "branch adı"` komutu ile yeni bir branch oluşturulur. `git branch -a` komutu ile branchler listelenir.

11- `git checkout "branch adı` ile yeni bir dala(branch) geçiş yapılabilir.

12- `git checkout --b "branch adı"` ile yeni bir branch oluşturulur ve o branche geçiş yapılır.

13- `git reset "commit_id" --soft` komutuyla tüm dosyalar staging area'dadır.

14- `git reset "commit_id" --hard` komutu ile id'si girilen commit'in oluşturulduğu düzene geri dönülür. Sonraki versiyonlar silinir.

15- `git branch -D "branch adı"` komutu branch silmek için kullanılır.

16-`git nerhe "branch adı"` ile verilen branch üstünde bulunan branch ile birleştiriliyor.




