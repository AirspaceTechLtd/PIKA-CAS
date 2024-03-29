# 皮卡丘数字证书颁发机构在线验证服务点

# Pikachu Certification Authority Online Service

## CA证书信息 / CA Certificates Details

> - **CN = Pikachu Root CA**
> - **O = Pikachu Trust Network CA**
> - **OU = Pikachu Certification Authority,  C  =  CN**
> - **Description = 皮卡丘数字证书信任系统根证书**

## 安装CA证书 / Import CA Certificates

> ### Win32 - [点击下载 / Download File](https://gitee.com/pikachuim/CA/raw/main/Import.zip)
>
> [Github海外](https://github.com/PIKACHUIM/CA/blob/main/Import.zip?raw=true)  [Gitee国内](https://gitee.com/pikachuim/CA/raw/main/Import.zip)  [CDN服务器](https://cdn-tx1.pika.net.cn/Cert/Import.zip)  [直链服务](https://cert.pika.net.cn/Import.zip)
>
> ```
> certutil.exe -urlcache -split -f "https://gitee.com/pikachuim/CA/raw/main/CA.zip" CA.zip
> 7z x -tzip -y CA.zip
> forfiles /p .\CA\ /s /c "cmd /c ..\certmgr.exe -add /all @path -s -r localMachine AuthRoot"
> forfiles /p .\CA\ /s /c "cmd /c echo @path"
> ```
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

## CA根证书 / Root CA - RSA-4096-SHA

> - ### **[证书信息 / Certificate Info]()**
>
>   - **证书算法(Signer Algorithm)：**`RSA4096(05 00) sha512RSA`
>
>   - **CA序列号(Certificate  SerN.)：**`4146d5c10b1a5e0ab0fc9432`
>
>   - **证书指纹(Certificate  SHA1)：**`31760fc0d2e3811fe217b4e499f51db02bf3a244`
> - ### [下载证书 / Download Cert]((CA-RSA.cer))
>
>   - **[CER](CA-RSA.cer)**   /  **[CRT](CA-RSA.crt)**   /  **[DER](CA-RSA.der)**   /  **[P7B](CA-RSA.p7b)**
>
> - ### **[吊销列表 / Revocation List](CA-RSA.crl)**
>
>   - [2020/01/01 - 2030/01/01](CA-RSA.crl)
>
>  - ### [中间证书 / Middle | Sub CA]()
>
>    - #### [Pikachu Sign Sub CA RSA](sign/CA-RSA.cer)
>
>      - **[CER](sign/CA-RSA.cer)**   /  **[CRT](sign/CA-RSA.crt)**   /  **[DER](sign/CA-RSA.der)**   /  **[P7B](sign/CA-RSA.p7b)**
>      - **[吊销列表 / Revocation  List](sign/CA-RSA.crl)**
>      
>    - #### [Pikachu Auth Sub CA RSA](auth/CA-RSA.cer)
>    
>      - **[CER](auth/CA-RSA.cer)**   /  **[CRT](auth/CA-RSA.crt)**   /  **[DER](auth/CA-RSA.der)**   /  **[P7B](auth/CA-RSA.p7b)**
>      - **[吊销列表 / Revocation  List](auth/CA-RSA.crl)**
>      
>    - #### [Pikachu File Sub CA RSA](file/CA-RSA.cer)
>    
>      - **[CER](file/CA-RSA.cer)**   /  **[CRT](file/CA-RSA.crt)**   /  **[DER](file/CA-RSA.der)**   /  **[P7B](file/CA-RSA.p7b)**
>      - **[吊销列表 / Revocation  List](file/CA-RSA.crl)**
>      
>    - #### [Pikachu Nets Sub CA RSA](nets/CA-RSA.cer)
>    
>      - **[CER](nets/CA-RSA.cer)**   /  **[CRT](nets/CA-RSA.crt)**   /  **[DER](nets/CA-RSA.der)**   /  **[P7B](nets/CA-RSA.p7b)**
>      - **[吊销列表 / Revocation  List](nets/CA-RSA.crl)**
