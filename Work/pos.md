pos接口：
	POS是Packet over SONET/SDH的缩写，是一种利用SONET/SDH提供的高速传输通道		SONET/SDH
	直接传送IP数据包的技术。POS技术支持光纤介质，他是一种高速先进的广域网连
	接技术。
	POS使用的链路层协议主要有PPP和HDLC。						链路层协议PPP HDLC
	POS接口的配置参数有接口带宽、接口地址、接口的链路层协议、接口的帧格式、		CSMA/CD（Carrier Sense Multiple Access
	接口的CRC校验和flag（帧中静负荷类型的标志位）等。					/Collision Detect）即载波监听
	IP ON SDH，简写POS，就是让IP在SDH的网上跑，其中，SDH是一种物理传输方式			多路访问/冲突检测机制
	IP网络是一种网络连接模式。							LLC 逻辑链路控制
											MAC 介质访问控制
The proper order of operation is:
	when transmitting:
	IP -> PPP -> FCS generation -> Byte stuffing -> Scrambling -> SONET/SD
	H framing

	when receiving:
	SONET/SDH framing -> Descrambling -> Byte destuffing -> FCS detection 
	-> PPP -> IP
