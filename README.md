conf t
aaa new-model
aaa authentication login default local
aaa authorization exec default local
aaa session-id common

netconf-yang
netconf-yang feature candidate-datastore
ip http server
ip http secure-server
restconf


gnxi
gnxi secure-init
service internal
gnxi secure-allow-self-signed-trustpoint
gnxi secure-password-auth
gnxi secure-server
gnxi server

end
write mem