# 皮卡丘数字证书颁发机构CA验证点

# Pikachu Certification Authority Online Service

## CA证书信息 / CA Certificates Identifiers

> - **CN = Pikachu Root CA XXX, O = Pikachu Trust Network CA**
>- **name = Pikachu Root CA XXX, 皮卡丘CA系统证书XXX**
> - **Description = 皮卡丘数字证书信任系统根证书**
> - **OU = Pikachu Certification Authority, C = CN**

## 安装CA证书 / Import CA Certificates

> ### Windows - [点击下载 / Download](https://github.com/PIKACHUIM/CA/raw/main/AUTO/ImportCA-Windows.zip)
>
> ### Linux - 导入方法 / Import Tutorial
>
> ```
> wget https://github.com/PIKACHUIM/CA/raw/main/CA.zip
> unzip CA.zip
> sudo cp -r CA/*.crt /usr/local/share/ca-certificates
> sudo update-ca-certificates
> sudo cp -r CA/*/*.crt /usr/local/share/ca-certificates
> sudo update-ca-certificates
> ```
>
> ### MacOS  - 导入方法 / Import Tutorial
>
> ```
> curl -L -o CA.zip -k "https://github.com/PIKACHUIM/CA/raw/main/CA.zip"
> unzip CA.zip
> for i in CA/*.cer; do
> echo "$i" && sudo security add-trusted-cert -d -r trustRoot "$i";
> done
> for i in CA/*/*.cer; do
> echo "$i" && sudo security add-trusted-cert -d -r trustRoot "$i";
> done
> ```

## [根证书 / Root CA - RSA-4096-SHA - 点击下载 / Download](CA-RSA.cer)

> - **证书信息 / Certificate Detail**
>   - 公钥算法(Public Key Algorithm)：**RSA4096(05 00)**
>   - 签名算法(Sign Algorithm)：**sha512RSA**
>   - 证书指纹(Cert SHA1)：**`a9a7334f32f10035a6bf2a9ae62671d29d2ddc3f`**
> - **[吊销列表 / Revocation List](CA-RSA.crl)**

## [根证书 / Root CA - ECC-P521-SHA - 点击下载 / Download](CA-ECCP521.cer)

> - **证书信息 / Certificate Detail**
>   - 公钥算法(Public Key Algorithm)：**ECDSA_P521**
>   - 签名算法(Sign Algorithm)：**sha512ECDSA**
>   - 证书指纹(Cert SHA1)：**`aafd6ef953a33e42aa7388e1a4cbc1174ecfb67c`**
> - **[吊销列表 / Revocation List](CA-ECCP521.crl)**

## [根证书 / Root CA - SM2-E256-SM3 - 点击下载 / Download](CA-SM2.cer)

> - **证书信息 / Certificate Detail**
>   - 公钥算法(Public Key Algorithm)：**SM2(1.2.156.10197.1.301)**
>   - 公钥参数(Public Key Parameters)：**06 08 2a 81 1c cf 55 01 82 2d**
>   - 签名算法(Sign Algorithm)：**SM3(1.2.156.10197.1.501)**
>   - 证书指纹(Cert SHA1)：**`ba8a72e9ddea14cd03d0bfc17c799ec7b2570661`**
> - **[吊销列表 / Revocation List](CA-SM2.crl)**

