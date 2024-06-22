
### Farcaster Node Hubble


### Linkler
 * [Memosr Twitter](https://twitter.com/memosrETH)
 * [Memosr Warpcast](https://warpcast.com/memosr)

 * Resmi döküman : https://www.thehubble.xyz/intro/hubble.html


## 🟢 Ön Bilgilendirme
- Bu işlem ile Farcaster üzerinde bir Node çalıştırabilirsiniz. 
- Bunu yapabilmek için Warpcast hesabınızın olması gerekiyor yoksa buradan üye olun 5$ maliyeti var
- https://warpcast.com/~/invite-page/450145?id=26f71802


## 🟢 özellik
- 16GB Ram fakat gözlemlediğime göre 16GB ram kullanmıyor daha az olabilir. Kurulumda 16GB istiyor 
- 4CPU
- 100Gb alan fazlasıyla yeter




## 🟢 Güncellemeler
```shell
sudo apt update -y
```

```shell
sudo apt upgrade -y
```

```shell
sudo apt install screen -y
```

```shell
screen -S warp
```



## 🟢 Docker indirelim	

```shell
sudo apt-get update
sudo apt-get install \
    ca-certificates \
    curl \
    gnupg \
    lsb-release
```

```shell
sudo mkdir -p /etc/apt/keyrings
curl -fsSL https://download.docker.com/linux/ubuntu/gpg | sudo gpg --dearmor -o /etc/apt/keyrings/docker.gpg

echo \
  "deb [arch=$(dpkg --print-architecture) signed-by=/etc/apt/keyrings/docker.gpg] https://download.docker.com/linux/ubuntu \
  $(lsb_release -cs) stable" | sudo tee /etc/apt/sources.list.d/docker.list > /dev/null
```


```shell
sudo apt-get update
```

```shell
sudo apt-get install docker-ce docker-ce-cli containerd.io docker-buildx-plugin docker-compose-plugin
```

```shell
sudo systemctl start docker
sudo systemctl enable docker
```

```shell
sudo curl -L "https://github.com/docker/compose/releases/download/v2.20.2/docker-compose-$(uname -s)-$(uname -m)" -o /usr/local/bin/docker-compose
```

```shell
sudo chmod +x /usr/local/bin/docker-compose
```


## 🟢 Tek kod kurulum çalıştıralım

```shell
curl -sSL https://download.thehubble.xyz/bootstrap.sh | bash
```

- Burada sizden ETH , OP mainnet ağında RPC isteyecek.  Bunu https://app.infura.io/dashboard ve https://www.alchemy.com/  buradan temin edebilirsiniz. 

#### 1-ETH mainnet RPC linkini girin
#### 2-Op Mainnet RPC linkini girin
#### 3-Warpcast FID numaranızı girin Profiliniz sağ üstten 3 çizgi ve About butonuna basın çıkıyor.

![image](https://hizliresim.com/f06cr3z)
![image](https://hizliresim.com/l2csxmt)


## 🟢 Sonuç izleme

- Aşağıdaki gibi çıktı almalısınız. Öncelikle Snap yükleyecek biraz uzun sürüyor ondan sonra resimdeki gibi bir ekran gelecek.

![image](https://github.com/HerculesNode/Testnet-Rehber/assets/101635385/80611013-b51f-4c52-9fed-1284357d430f)


- Ayrıca grafana ile kontrol edebilirsiniz.  http://SUNUCU-IP:3000 şeklinde

![image](https://github.com/HerculesNode/Testnet-Rehber/assets/101635385/1496c07d-c8b2-44ec-86ae-6b5fcada0526)


