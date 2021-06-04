# Guide of Tuya Firmware burning authorizations for ESP8266

## **Prerequisites**

1.Ensure that your system meets the requirements of the installation environment:

- **System:** Support only 32-bit or 64-bit Windows 7 or above operating system.
- **Hard disk:** The system disk (disk C) reserves more than 200 MB storage space.
- **Memory:** More than 1 GB of memory space is required to ensure stable software operation.
- **Processor:** Core i5 or above is required to ensure stable software operation.
- **Runtime library:** .Net Framework 4.0 runtime library. In general, related libraries are preinstalled in the system.

2.Download the installation packages on Google drive:[Installation Packages](https://drive.google.com/file/d/1SF-rM5qDLaPJiuMHrkqFauVyRXSSHMkj/view?usp=sharing).

## **Step1: Create a product and get your token ID**

To implement the communication between an Arduino-compatible board and ESP8266, you need to create a product on the [Tuya IoT Platform](https://iot.tuya.com/?_source=ccbb5041db8e537eb005ee8dce8b70d8) beforehand to get the product ID (PID) and **send your Tuya IoT Account and PID to** [devops@tuya.com](devops@tuya.com)**to get your Token ID.**

For example, the steps to get the PID of a smart light bulb are as follows:

1.Log in to the [Tuya IoT Platform](https://iot.tuya.com/?_source=ccbb5041db8e537eb005ee8dce8b70d8).

2.See [Create Products](https://developer.tuya.com/en/docs/iot/configure-in-platform/create-product/create-product?id=K914jp1ijtsfe) and create a smart light bulb product, such as a Wi-Fi and Bluetooth Low Energy light bulb implemented by the **Custom Solution**.

​            ![img](https://wdcdn.qpic.cn/MTY4ODg1MDI5OTc1MTU0MA_98445_z15VKr6xpjTUnqfl_1622537406?sign=1622793067-1098864985-0-dfc249c0f64fb99722f2ba11f7f3e7f3)            

3.Copy the PID and send it to [devops@tuya.com](devops@tuya.com)together with your Tuya IoT account name to get your Token ID.

​            ![img](https://wdcdn.qpic.cn/MTY4ODg1MDI5OTc1MTU0MA_141539_yiCzfG1entSTaR4D_1622537406?sign=1622793067-889732388-0-08ad5e9320af9dfe4ec6ffb5f57de7e9)            

## 

## **Step2: Register PMS and activate your Token ID**

1.Sign up the [PMS System](https://pms.tuya.com/en/login?_source=13efde86f8c2306108c691615a0ff592). and login

​            ![img](https://wdcdn.qpic.cn/MTY4ODg1MDI5OTc1MTU0MA_799440_-yuTVs4o5Z2FYN0H_1622541080?sign=1622793067-1957239040-0-f1d8d9822aa19fa9a1dc6e2ae3ff5518)            

2.Select Factory Work Order-Activation Code Verification.Input Token ID that you got from Step1 and confirm.One Token ID can only be activated by one user.

​            ![img](https://wdcdn.qpic.cn/MTY4ODg1MDI5OTc1MTU0MA_906761_d4R-Y3cerFEHqHot_1622539016?sign=1622793067-2115171135-0-48eb5ca64205453d12ca94139ca5503d)            

​            ![img](https://wdcdn.qpic.cn/MTY4ODg1MDI5OTc1MTU0MA_292903_2MXVDOb-ztwHT5c3_1622539221?sign=1622793067-1241243775-0-61429e480dc679ec9bc6291cc008fd93)            

## **Step3: Install TYDA.exe and ESP8266 driver**

## 1.Download installations package on the goolge drive:[Installation Packages](https://drive.google.com/file/d/1SF-rM5qDLaPJiuMHrkqFauVyRXSSHMkj/view?usp=sharing).Install the Tuya_TYDA_Install_V2.4.0 and login with your PMS account.And then click **Online Login**. You can choose **Automatic Login** and **Remember The Password** as needed.            ![img](https://wdcdn.qpic.cn/MTY4ODg1MDI5OTc1MTU0MA_964731_lSPvV28fVl6XI426_1622540841?sign=1622793067-1936010714-0-3b5467f4a41730cfb97703faba288480)            

​            ![img](https://wdcdn.qpic.cn/MTY4ODg1MDI5OTc1MTU0MA_35721_Xxh0BuJNM7sRoEjf_1622541194?sign=1622793067-1517377812-0-e3469255bfae162c96eda55143f4b455)            

2.You must set up Burning Baud and click **Ok** for the first time setup.

​            ![img](https://wdcdn.qpic.cn/MTY4ODg1MDI5OTc1MTU0MA_944052_LAC8vqOUPzl5Kgeh_1622541595?sign=1622793067-875234491-0-bc4371b5e072f480b0c626bc67fb9fe3)            

​            ![img](https://wdcdn.qpic.cn/MTY4ODg1MDI5OTc1MTU0MA_399248_wvvlLX_kqg9zxWw5_1622541683?sign=1622793067-1735812612-0-00da2465247c076ad2b27f4525730097)            3.Insert the USB interface of ESP8266 to your PC and install ESP8266 driver CP210x.

​            ![img](https://wdcdn.qpic.cn/MTY4ODg1MDI5OTc1MTU0MA_734314_EHt-H-KmgsTV0-AS_1622542052?sign=1622793067-492742480-0-8e33d0655640822b4f92be839deddd5a)                        ![img](https://wdcdn.qpic.cn/MTY4ODg1MDI5OTc1MTU0MA_769872_GkHFxs2Zz79s7-8z_1622542100?sign=1622793067-303934701-0-d356fbbfaea8f951939ecf6a2689bf50)            

​            ![img](https://wdcdn.qpic.cn/MTY4ODg1MDI5OTc1MTU0MA_56200_amlpQlXLVGAPt4Zi_1622542224?sign=1622793067-510578838-0-bbe828d28d1ee9e167b3b727b792029a)            

## **Step4: Enter Token and Run the buring**

1.Click **Enter Token** to input the token and select work station-Buring Authorization

​            ![img](https://wdcdn.qpic.cn/MTY4ODg1MDI5OTc1MTU0MA_550666_t3DIsBHiU8teQ4E__1622542371?sign=1622793067-129642166-0-afb303d66a9b7fcae627055cfeaef4fe)            

​            ![img](https://wdcdn.qpic.cn/MTY4ODg1MDI5OTc1MTU0MA_193091_Q9CGFECFCbBk7wDh_1622542414?sign=1622793067-1453098685-0-6657dde2bbcb9814cb4e1a0bcd0ba5c1)            2.Then click **OK**. The following page is displayed.

​            ![img](https://wdcdn.qpic.cn/MTY4ODg1MDI5OTc1MTU0MA_342336_jIaqI7KZJAjFXAHQ_1622542739?sign=1622793067-2029043656-0-82437e3fd84d9ae901647dc202f19287)            

3.Then click **RUN**. The burning is starting until 100%.

​            ![img](https://wdcdn.qpic.cn/MTY4ODg1MDI5OTc1MTU0MA_404105_A2RSKOdIV5HROQJg_1622542831?sign=1622793067-952574128-0-466fdf065859c5617773d0e6007ef475)            

​            ![img](https://wdcdn.qpic.cn/MTY4ODg1MDI5OTc1MTU0MA_207252_vr_EOtD41rB-Tgh7_1622542932?sign=1622793067-178909625-0-8ab43686479f07bed8d0289a40929a23)            

**And you succeed!** 