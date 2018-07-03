# DPDKstats
vRouter DPDK statistics collect the sript

./dpdkstats.py  
  Options:
  
  -v VIF, --vif VIF     vif number - only number after vif0/
  
  -t TIME, --time TIME  time for test default 3 seconds
  
  -c CPU, --cpu CPU     number of CPUs assigned to vRouter - default will be autodetected
  
  -all, --all_vifs      total CPU utilisation from all VIFs
  
  # Example of use 
  Show total CPU utilisation

```
./dpdkstats.py --time 5 --cpu 6 --all_vifs
----------------------------------
|         pps per Core           |
----------------------------------
|Core 0  |TX + RX pps: 520033    |
|Core 1  |TX + RX pps: 372574    |
|Core 2  |TX + RX pps: 478116    |
|Core 3  |TX + RX pps: 420974    |
|Core 4  |TX + RX pps: 487320    |
|Core 5  |TX + RX pps: 480913    |
----------------------------------
| Total  | pps: 2759930          |
----------------------------------



./dpdkstats.py --time 5 --cpu 6 --vif 0
-------------------------------------------------------------------------------------------------------------------------------------
|Core 1  | TX pps: 283737    | RX pps: 236696    | TX bps: 423580648 | RX bps: 353133107 | TX error: 0         | RX error 0         |
-------------------------------------------------------------------------------------------------------------------------------------
|Core 2  | TX pps: 136609    | RX pps: 235524    | TX bps: 201346001 | RX bps: 351291254 | TX error: 0         | RX error 0         |
-------------------------------------------------------------------------------------------------------------------------------------
|Core 3  | TX pps: 238158    | RX pps: 236921    | TX bps: 359514034 | RX bps: 353319124 | TX error: 0         | RX error 0         |
-------------------------------------------------------------------------------------------------------------------------------------
|Core 4  | TX pps: 181262    | RX pps: 239014    | TX bps: 268611209 | RX bps: 356478849 | TX error: 0         | RX error 0         |
-------------------------------------------------------------------------------------------------------------------------------------
|Core 5  | TX pps: 266889    | RX pps: 219515    | TX bps: 397977590 | RX bps: 327308671 | TX error: 0         | RX error 0         |
-------------------------------------------------------------------------------------------------------------------------------------
|Core 6  | TX pps: 269471    | RX pps: 210458    | TX bps: 401873006 | RX bps: 313822642 | TX error: 0         | RX error 0         |
-------------------------------------------------------------------------------------------------------------------------------------
|Total   | TX pps: 1376126   | RX pps: 1378128   | TX bps: 2052902488| RX bps: 2055353647| TX error: 0         | RX error 0         |
-------------------------------------------------------------------------------------------------------------------------------------
```

 
