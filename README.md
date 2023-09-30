# subsquidNode Kurulum Rehberi - Hercules
![image](https://github.com/herculessx/subsquidNode/assets/101635385/b0e1aa8a-4e2b-4720-893f-b2786ab4529c)

 ## 🟢 Linkler:

 * [squids](https://app.subsquid.io/squids/)
 * [Başvuru Formu](https://subsquid.deform.cc/testnetnodeapplication/)
 * [Hercules Telegram](https://t.me/HerculesNode)
 * [Hercules Twitter](https://twitter.com/Herculesnode)


 ## 🟢 Ödül sistemi

 Node Çalıştıran ve Uygulama yoluyla seçilen en fazla 500 katılımcı  en üst sıradaki 133 node ödüller için uygun olacaktır.

 Diğer Testnet Katılımcıları: Sınırsız; üst sıralarda yer alan 4.000 ödül için uygun olacak

 Testnet 4 ay sürmesi bekleniyor

 Token arzının % 2'si  26.600.000 SQD ödül olarak dağıtılacak.

## 🟢 Sistem Gereksinimleri

* 4 CPU
* 8GB RAM
* 1TB DISK
* Ubuntu 20.04+


## 🟢 Kurulum



```shell
sudo apt update -y && sudo apt upgrade -y
```

```shell
apt install npm
```

```shell
sudo npm install -g npm@10.1.0
```

<hr>

```shell
curl -sL https://deb.nodesource.com/setup_20.x | sudo -E bash -
```
Biraz bekleyelim  (Bu kodu TestNetrun rehberinden alıntıladım. Teşekkürler kendilerine)
<br><hr>



```shell
sudo apt-get install -y nodejs
```

<hr>

Bu adrese gidelim [ Dashboard](https://app.subsquid.io/squids/)   
  
1- Install the CLI

```shell
npm install -g @subsquid/cli
```
![image](https://github.com/herculessx/subsquidNode/assets/101635385/5f3440d8-53a7-4aba-bcdc-23846e5dcc1a)


2- Configure the CLI  Burası herkeste değişiyor 2. kodu kopyalayın.

![image](https://github.com/herculessx/subsquidNode/assets/101635385/9836e6c9-805e-4740-9f84-2633189ef156)


2. Set up your squid 

* Buraya isminizi yazın küçük harflerle 

![image](https://github.com/herculessx/subsquidNode/assets/101635385/0b16cba4-6793-4ac3-b849-5afa89711a99)


```shell
apt install git
```

Init Squid directory olan kodu girin. isminizi yazınca otomatik oda değişiyor

Burada isminizin olduğu kodu girin. Aşağıdaki gibi bir çıktı almanız lazım

![image](https://github.com/herculessx/subsquidNode/assets/101635385/91d69e8e-c3e6-478e-ae00-506e7912eb09)


En alttaki deploy kodunu girin ve kurulum başlıyor.


![image](https://github.com/herculessx/subsquidNode/assets/101635385/bebf4c73-b9ac-460d-b29f-24e0478efd03)


Dashboard kısmına gidin ve ardından panel açılacak sync olmasını bekleyelim şimdilik bu kadar. Resimdeki gibi olması gerekiyor

![image](https://github.com/herculessx/subsquidNode/assets/101635385/1e3f3097-b5f8-4879-a15e-5d10c653d695)



## 🟢 Ankr Hata Çözümü

src/processor.ts  dosyasını açın chain bölümünde ankr göreceksiniz bunu Alchemy yada başka bir yerden aldığınız bir RPC ile değiştirin ve kaydedin

![image](https://github.com/herculessx/subsquidNode/assets/101635385/777ff06c-d610-4ff0-a760-808b852e797b)

Ardından deploy etmemiz gerekiyor  Aşağıdaki kodu çalıştırın isminiz yazan yerlere klasör isminiz ne ise onu yazın 


```shell
sqd deploy --org isminiz ./isminiz
```

![image](https://github.com/herculessx/subsquidNode/assets/101635385/69d5290a-1b48-4a94-b175-25c0b629b089)


## 🟢 Suck sorunu ( isminiz kısmını değiştirin hesap isminiz ile )

```shell
sqd restart isminiz@v1
```

![image](https://github.com/herculessx/subsquidNode/assets/101635385/8af61c81-5c6c-4834-a69b-5a31ec5587a1)


## 🟢 Log bakmak için  ( isminiz yazan yeri değiştirin )

```shell
npx sqd squid:logs isminiz@v1 -f
```



