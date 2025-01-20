

# SO HOW DOES A WEBRTC WORK ? MORE SPECIFICALLY HOW REAL TIME MEDIA COMMUNICATION HAPPENS

two clients or multiple clients exhannge their ips with each other so they can know where to send the video packets
they send the video packets through a p2p comm protocol

now the p2p comm is made as follows >>

first the client 1 sends a request to a STUN server .. saying the STUN server whats's my request coming from is it a public ip or private ip
base on that the stun server responds with ice canditates (they are the ip addresses that can be shared with another client to receive or send media)

the clien2 does the same thing 

so both of the client have their ice candidates and they send it to a signalling server

what the signalling server does is >

the client sends the signaling server their ice candidates and the server sends it to another client , this happens for both of the clients