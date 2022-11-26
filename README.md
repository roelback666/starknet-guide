# Guide Starknet Testnet

<p style="font-size:14px" align="right">
<a href="https://t.me/moli1337" target="_blank">Telegram<img src="https://user-images.githubusercontent.com/50621007/183283867-56b4d69f-bc6e-4939-b00a-72aa019d1aea.png" width="30"/></a>
<p align="center">
  <img height="auto" width="auto" src="https://580801350-files.gitbook.io/~/files/v0/b/gitbook-x-prod.appspot.com/o/spaces%2FI3uyPQUnfzoZEU60Wqmq%2Fuploads%2FWVpVjjbonJcxSAt43p7I%2FSTRAKNNNN.jpg?alt=media&token=c52b93f8-fa32-458f-a09b-7b655dc650c6">
</p>


## Referensi

[Twitter](https://twitter.com/StarkWareLtd)

[Server Discord ](https://discord.gg/qypnmzkhbc)

[Explorer](https://voyager.online/)

# Register Alchemy

1. [Dattar Disni](https://alchemy.com/?r=35f2a3b3d541aee8)

2. Buat App
 - Pilih Ethereum Mainnet
 <p align="center">
  <img height="auto" width="auto" src="https://i.ibb.co/Nrd73jP/Screenshot-11.png">
</p>

 - Masuk ke App -> Pilih View Key -> Salin HTTPS , Simpan di Notepad.
  <p align="center">
  <img height="auto" width="auto" src="https://i.ibb.co/5297Q1s/Screenshot-12.png">
</p>

*DI CEK LAGI ETHEREUM MAINNET
## KEMBALI KE VPS
- Install Docker , alat , dan bahan2.
```
sudo apt update -y && sudo apt install apt-transport-https ca-certificates curl software-properties-common -y && curl -fsSL https://download.docker.com/linux/ubuntu/gpg | sudo apt-key add - && sudo add-apt-repository "deb [arch=amd64] https://download.docker.com/linux/ubuntu focal stable" && sudo apt install docker-ce
sudo apt-get install -y pkg-config curl git build-essential libssl-dev screen
git clone --branch v0.4.0 https://github.com/eqlabs/pathfinder.git
```
## Running Node
```
mkdir -p $HOME/pathfinder docker run -d
--rm
-p 9545:9545
--user "$(id -u):$(id -g)"
-e RUST_LOG=info
--name starknet
-e PATHFINDER_ETHEREUM_API_URL="https://eth-mainnet.g.alchemy.com/v2/HE50Y4MAEZ4KM1-ud4465hs6"
-v $HOME/pathfinder:/usr/share/pathfinder/data
eqlabs/pathfinder

mkdir -p $HOME/pathfinder
docker run -d \
  --rm \
  -p 9545:9545 \
  --user "$(id -u):$(id -g)" \
  -e RUST_LOG=info \
  --name starknet \
  -e PATHFINDER_ETHEREUM_API_URL="XXXXXXXXXXXXX" \
  -v $HOME/pathfinder:/usr/share/pathfinder/data \
  eqlabs/pathfinder
  ```
`"XXXXXXXXXXXXX"` Ganti dengan HTTPS alchemy Kalian.

- Example 
```
mkdir -p $HOME/pathfinder docker run -d
--rm
-p 9545:9545
--user "$(id -u):$(id -g)"
-e RUST_LOG=info
--name starknet
-e PATHFINDER_ETHEREUM_API_URL="https://eth-goerli.g.alchemy.com/v2/lkgcLd5qefY8bNOySMvrIO-eozZs6zUt"
-v $HOME/pathfinder:/usr/share/pathfinder/data
eqlabs/pathfinder
```

## Cek Logs

```
docker logs -f starknet
```

  <p align="center">
  <img height="auto" width="auto" src="https://i.ibb.co/PmsBjsh/Screenshot-13.png">
</p>
 
 ## Cek Last Block
 
 [DISINI](https://voyager.online)
 
 
 ## Tugas Terakhir
 
 - Screenshot Dashboard Alchemy.
 
   <p align="center">
  <img height="auto" width="auto" src="https://i.ibb.co/GWKVCbb/Screenshot-14.png">
</p>

- Post Twitter + Salin link tweet nya.

- Kirim ke Discord #✅｜full-node-success. ( feedback , IP VPS , Link Tweet , SS dari dashboard alchemy )

   <p align="center">
  <img height="auto" width="auto" src="https://i.ibb.co/0DjLxsS/Screenshot-16.png">
</p>

 
 
 
 
 
 
