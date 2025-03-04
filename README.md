During this, the board listened to the telnet port, and the telnet port had been set to 23.
and board echoed back to the special IP address that was 192.168.1.15 and netmask:255.255.255.0.
With the putty, received data on the telnet port had been illustrated.
For extra learning, you can set a password or answer key in a given part of the echo.c code.
/* indicate that the packet has been received */
	tcp_recved(tpcb, p->len);

	/* echo back the payload */
	/* in this case, we assume that the payload is < TCP_SND_BUF */
	if (tcp_sndbuf(tpcb) > p->len) {
		err = tcp_write(tpcb, p->payload, p->len, 1);
	} else
		xil_printf("no space in tcp_sndbuf\n\r");
How do it? It is your own.
