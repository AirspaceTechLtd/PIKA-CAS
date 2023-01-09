# 皮卡丘数字证书颁发机构CA验证点
## Pikachu Certification Authority Online Service

## CA证书信息 / CA Certificates Identifiers

> - **CN = Pikachu Root CA RSA, O = Pikachu Trust Network CA**
>- **name = Pikachu Root CA RSA, 皮卡丘CA系统证书RSA**
> - **Description = 皮卡丘数字证书信任系统根证书**
> - **OU = Pikachu Certification Authority, C = CN**

## 自动安装证书 / Auto Import CA Certificates

> ### Windows - [点击下载 / Download](AutoCA.exe)
>
> ### Linux - `curl xxxxxxxxxxxxxxxx`
>
> ### MacOS - `curl xxxxxxxxxxxxxxxx`

## [根证书 / Root CA - RSA-4096-SHA](CA-RSA.cer)

> - **证书信息 / Certificate Detail**
>   - 公钥算法(Public Key Algorithm)：**RSA(05 00)**
>   - 签名算法(Sign Algorithm)：**sha512RSA**
>   - 证书指纹(Cert SHA1)：**`a9a7334f32f10035a6bf2a9ae62671d29d2ddc3f`**
> - **[吊销列表 / Revocation List](CA-RSA.crl)**

## [根证书 / Root CA - ECC-E512-SHA](CA-ECC.cer)

> - **证书信息 / Certificate Detail**
>   - 公钥算法(Public Key Algorithm)：**brainpoolP512t1**
>   - 签名算法(Sign Algorithm)：**sha512ECDSA**
>   - 证书指纹(Cert SHA1)：**`79b513c611670d9e5120325be6800fb1fde03bd9`**
> - **[吊销列表 / Revocation List](CA-ECC.crl)**

## [根证书 / Root CA - SM2-E256-SM3](CA-SM2.cer)

> - **证书信息 / Certificate Detail**
>   - 公钥算法(Public Key Algorithm)：**SM2(1.2.156.10197.1.301)**
>   - 公钥参数(Public Key Parameters)：**06 08 2a 81 1c cf 55 01 82 2d**
>   - 签名算法(Sign Algorithm)：**SM3(1.2.156.10197.1.501)**
>   - 证书指纹(Cert SHA1)：**`ba8a72e9ddea14cd03d0bfc17c799ec7b2570661`**
> - **[吊销列表 / Revocation List](CA-SM2.crl)**

