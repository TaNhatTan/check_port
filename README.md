# check_port
 ---------------------------------------------------
        A simple, fast, lightweight TCP/UDP scanner

Usage: ./piescan.py -t [targets] -p [ports] [options]

Options:

        -t         [target ip]                   
    	-p         [port]                         Examples: ( -p 25 || -p 22,23,24,25 || -p 0-1024 )
    	-s[TU]     Scan type ( default = -sT )    Examples: ( -sT : TCP || -sU : UDP )    
    	-v         Verbose output                
    	--timeout  [timeout in ms]               

Examples:

        ./piescan.py -sT -t 127.0.0.1 -p 0-65535 -v  - Do a verbose TCP scan of all ports on 127.0.0.1
        ./piescan.py -sU -t 127.0.0.1 -p 0-100       - Do a UDP scan of the first 100 ports on 127.0.0.1
