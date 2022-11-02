# 数字证书验证点
- ## 皮卡丘数字证书系统

  - ### [根证书 - RSA-4096-SHA](PikaRoot/CA.cer)

    > **Description = 皮卡丘数字证书系统根证书**
    > **Description = Pikachu Digital Certificate System Root CA**
    > **CN = Pikachu Root CA**
    > **OU = Certificate Management**
    > **O = Pikachu Group**
    > **L = Yongchuan**
    > **S = Chongqing**
    > **C = CN**
    >
    > [吊销列表](PikaRoot/CRL/CA.crl)

    - #### 

  - ### [根证书 - SM2-E256-SM3](PikaRoot/CA-SM2.cer)

- ## 极客邦数字证书系统

  - ### [根证书 - RSA-4096-SHA](GeekBang/CA.cer)

    > **Description = 四川大学智能感知与先进控制实验室**
    > **Description = Intelligent Perception and Advanced Control Lab., SCU**
    > **Description = 四川大学极客邦**
    > **Description = GeekBang of Sichuan University**
    > **CN = SCU GeekBang Root CA**
    > **OU = Certificate Management**
    > **O = SCU GeekBang**
    > **L = Chengdu**
    > **S = Sichuan**
    > **C = CN**
    >
    > [吊销列表](GeekBang/CRL/CA.crl)

  - #### [中间证书 - SCU GeekBang Tunnel Sub CA](GeekBang/TSC.cer)

    > **Description = GeekBang Network Tunnel Root Certificate**
    > **Description = 极客邦网络隧道根证书**
    > **CN = SCU GeekBang Tunnel Sub CA**
    > **OU = Network Management**
    > **O = SCU GeekBang**
    > **L = Chengdu**
    > **S = Sichuan**
    > **C = CN**
    >
    > [吊销列表](GeekBang/CRL/TSC.crl)

    - ##### [中间证书 - SCU GeekBang MainRouter VPN Server](GeekBang/MR-VPNS.cer)

      > **CN = SCU GeekBang MainRouter VPN Server**
      > **OU = Network Management**
      > **O = SCU GeekBang**
      > **L = Chengdu**
      > **S = Sichuan**
      > **C = CN**
      >
      > [吊销列表](GeekBang/CRL/MR-VPNS.crl)

    - 

  - 

- ### [根证书 - SM2-E256-SM3](GeekBang/CA-SM2.cer)
