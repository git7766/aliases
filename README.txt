echo "be smart 
typing:
start"
# basic_aliases
# basic_navigation
# basic_installs
# using_apps
# system_acctions
# back_up_playground_pen
# important_commands



alias start='
    echo "###########################################################"
    echo "# ___ HELLO EVERYONE ___ i have many useful aliases       #"
    echo "#                        for you;                         #" 
    echo "#                     this aliases will be helpful        #"    
    echo "#                                                         #"
    echo "#       => show// for_basic:                              #"
    echo "#             // * aliases                                #"
    echo "#            // * navigation                              #"    
    echo "#           // * installs                                 #"
    echo "#            for other:                                   #"
    echo "#         // * using apps                                 #"
    echo "#        // * systems acctions                            #"
    echo "#       => back_ups//                                     #"
    echo "#       => show_commands// for important commands         #"
    echo "#  /////////////////////////////////////////////////////  #"
    echo "#       - // this is commend                              #"
    echo "#       - => this is alias, and can you typing it         #"
    echo "#       typing for example:                               #"
    echo "#       show                                              #"
    
    
    '



alias show='
    echo "###########################################################"
    echo "# ___ HELLO EVERYONE ___ look what I have ___             #"
    echo "# basic_aliases::                                         #"
    echo "#     // :: information                                   #"
    echo "#       => check_core//                                   #"
    echo "#                                                         #"
    echo "#       => aliases// open ~/.bash_aliases                 #"
    echo "#       => blinding// code .../.l64.../.bash_aliases      #"
    #cho "#                                                         #"
    echo "# basic_system::                                          #"
    echo "#     // ::information                                    #"
    echo "#       => check_core// sudo lshw | grep core             #"
    echo "#                                                         #"
    echo "# basic_navigation::                                      #"
    echo "#       => playground// cd /media/*/.l64/playground       #"
    echo "#                                                         #"
    echo "# basic_install::                                         #"
    echo "#     // ::mac_address                                    #"
    echo "#       => install_macchanger                             #"
    echo "#                                                         #"
    echo "#       => install_snapd                                  #"
    echo "#     // ::optimalization                                 #"
    echo "#       => install_xfce4                                  #"
    echo "#     // ::browsers                                       #"
    echo "#       => install_chrome                                 #"
    echo "#       => install_opera                                  #"
    echo "#                                                         #"
    echo "# using_apps::                                            #"
    echo "#     // ::mac_address                                    #"
    echo "#       => macchanger_alt// if you have error             #"
    echo "#       => macchanger_r                                   #"
    echo "#     // ::browsers_using_apps::                          #"
    echo "#       => t// open .l64/tor                              #"
    echo "#                                                         #"
    echo "# system_acctions::                                       #"
    echo "#       => suspend//   systemctl suspend                  #"
    echo "#       => hibernate// systemctl hibernate                #"
    echo "#       => down//      shutdown -h now                    #"
    echo "#                                                         #"
    echo "# back_ups::                                              #" 
    echo "#       => back_up_playground_pen //                      #" 

    '



alias back_ups='
    echo "###########################################################"
    echo "# ___ HELLO EVERYONE ___ THIS ARE SYSTEM BUCK_UP WITH PEN #"
    echo "#                                                         #"
    echo "#     // ::playground                                     #"
    echo "#       => back_up_playground_pen// all                       
    '


alias show_commands='
    echo "###########################################################"
    echo "# ___ HELLO EVERYONE ___ THIS ARE BEST IMPORTANT COMMANDS #"
    echo "#                                                         #"
    echo "# tar xvf xxx.tar.xz// open file //str.244                #"

    '





#####################################################################
# basic_aliases::
# ln -s
alias blinding='
        ln -s /media/*/.l64/playground/.bash_aliases ~/
    '
alias aliases='
        code /media/*/.l64/playground/.bash_aliases || open /media/*/.l64/playground/.bash_aliases
    '




#####################################################################
# this is basic_navigation::
alias playground='
        cd /media/*/.l64/playground
    '

#####################################################################
# basic_system::

        
    #basic_system_information
        alias check_core='
            sudo lshw | grep core
        '
#####################################################################
# install::
    #install_mac_address
        alias install_macchanger='
                sudo apt install macchanger
            '
            # if it's proglem with changes mac:
            # [error] ...: device or resource busy
            # have to use macchanger_alt 

alias install_snapd='
        sudo apt install snapd
    '
    #basic_system_optimalization
            # przy logowaniu wybieram srodowisko
        alias install_xfce4='
                sudo apt install xfce4
        '

    #installs_browsers
        alias install_chrome='

            '
        alias install_opera='
                sudo snap install opera
            '





#####################################################################
# using_apps::
    #using_apps_mac_address
        alias macchanger_r='
                sudo macchanger -r wlp62s0
            '
        alias macchanger_alt='
                sudo service NetworkManager stop; 
                    
                    echo "for wlp62s0 - hp"
                    sleep 1s;
                    sudo ifconfig wlp62s0 down;
                    sudo macchanger -r wlp62s0;
                    sudo ifconfig wlp62s0 up;
                        
                        echo "for enp0s25 - hp"
                        sleep 1s;
                        sudo ifconfig enp0s25 down;
                        sudo macchanger -r enp0s25;
                        sudo ifconfig enp0s25 up;

		    echo "for enp2s0 - pc"
		    sleep 1s;
		    sudo ifconfig enp2s0 down;
		    sudo macchanger -r enp2s0;
		    sudo ifconfig enp2s0 up;
		    
		        echo "for enp4s0 - pc"
		        sleep 1s;
		        sudo ifconfig enp4s0 down;
		        sudo macchanger -r enp4s0;
		        sudo ifconfig enp4s0 up;

                sudo service NetworkManager start ;
            '
    #using_apps_browser_using_apps
        alias t='
                cd /media/m/.l64/playground/tools/browsers/tor-browser/; ./start*
            '




#####################################################################
# system_acctions::
alias suspend='
        systemctl suspend
    '

alias hibernate='
        systemctl hibernate
    '

alias down='
        shutdown -h now
    '

######################################################################
# back_ups::
    #back_ups_playground
        alias back_up_playground_pen='
            rm -r /media/*/.l64/back_ups/playground;
            cp -riv /media/*/.l64/playground /media/*/.l64/back_ups
        '
        
        
## check the linux version 
## cat /etc/lsb-release
## more spcecivication:
## 	xdg-open "https://www.howtouselinux.com/post/check-linux-version"
