# OSCP_cheatcheet
Tenbird-OSCP

NMAP
  자주사용하는것 nmap -sT -sV -Pn -T5 --open {ip} <br>
-sS : TCP SYN 스캔 (root권한 필요하며, 속도는 빠르지만 DOS 공격을 일으킬 수 있음)<br>
-sU : UDP 스캔 (SNMP 네트워크 서비스 확인 필요)<br>
-sT  : TCP CONNECT 스캔(기본)<br>
-p : 포트 지정<br>
-Pn : ICMP 요청, 포트 80 등 기본적인 포트스캔 비활성화 (적은 패킷으로 더 빠르게 확인 가능)<br>
-n : dns 질의 안함<br>
--open : 열린 포트만 출력<br>
-p- : 1 to 65535 포트 대상<br>
-T3 : default 속도로 T5가 가장 빠르지만, 패킷 손실이 있을 수 있음<br>
--min-rate 2000 : 최소 매초 2000개의 패킷 전달 <br>
-oA : 출력 결과 저장<br>
-sC : 스크립트 기반 스캔<br>
-sV : 서비스 버전 정보 확인<br>
-A : (-o(OS탐지), -sV, -sC, --traceroute) 포함으로 네트워크 부하를 줄 수 있어서 권장하지 않음.<br>
