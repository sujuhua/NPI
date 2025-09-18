# __GS001_S1__
* *测试工序*：__晶圆厂MAP导入——CP1测试(常温25℃)——充氮烘烤（24小时@250℃）——CP2测试(常温25℃)——UV光照(45mins@波长253nm，功率20mW/cm2)——CP3测试(高温135℃)——AOI——MAP出货__

## __CP__

    1. INIT测试项增加BOR初值测试；
    2. 增加DVS测试 ，等待DVS方案
    3. 高温测NLD漏电数据提供给林理乾
    4. 关于回收和分BIN：OTP不良
## __FT__
    1. OTP 回收 ：fail写下一个block
    2. CAN修调方案优化
    3. DSI调挡位问题 换挡位没变化
    4. pwm捕获/输出测试波形某一个即可
    5. DSI3调试
    6. 漏电测试数据和ADC0内部通道扫描结果数据整理发给林理乾

# __GB003__
* 产品型号 ` BF8816A，BF8916A`；
* 测试工序： 
* 程序:
    ```
    BF8916A_FT_8SITE_LT_V1.flw
        BF8916A_FT_8SITE_HT_V1.flw
        BF8916A_FT_8SITE_RT_V1.flw
        BF8916A_FT_8SITE_QC_V1.flw
    ```
## __FT task__

### 已完成：
    1. RT修调中心值上调offset，VD5,VREF，ADC转换5V ->5.06V；
    2.0908 评审，待解决

### `未完成`：
    1.CnSn_near漏电测试卡控C0S0为3uA，其余为2uA；
    3.BGV修调测试确认，无修调，需使能，测量结果RT和QC有差；
    4.借机利扬，压测不良品然后寄回应用谢喜克，然后机台反复跑料验证是否会打坏芯片；
    5.测试时间采集和优化；
    6.同8815，查看是否增加了线性回归测试，极值卡控，ADOL测
    7.QC存在FUN测试低良和TRIM RETEST低良;
    8.温漂梳理升级

---
# __BMS01/BMS02__

*note*:
* BMS01A?
* BMS01B、BMS01C(BF8815A、BF8915A)：BMS01C和BMS01B的晶圆型号不同，FT名称一样
* BMS02B、BMS02C（BF8815B、BF8915B）：BMS02C和BMS02B的晶圆型号不同，FT名称一样

* 异物检测和DIODE都需要删除

## __BMS01A__
```
1. 需输出《文档》
```

## __BMS01B/BMS01C__
FT产品型号BF8815A,BF8915A,三温测试程序
