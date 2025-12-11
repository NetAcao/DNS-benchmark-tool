# DNS-benchmark-tool
To find the fastest (lowest latency) for your DNS server
Automated DNS Latency Tester script

While working on a project to set up a local DNS server on a Raspberry Pi, I wanted to identify the fastest DNS resolvers available. Initially, I considered manually pinging each DNS server to compare their performance, but I decided to automate the process. I created a short script using Python with some help of AI, to ping a list of preconfigure public DNS servers and calculate their minimum, maximum, and average latency. The script also identifies and recommends the top 3 fastest DNS servers for use with the local DNS server. I will share this script as an open-source project on GitHub for others to use and contribute to.

The script is designed to work seamlessly on both Windows and Linux (or macOS) systems. The only difference lies in the ping command:
For Windows, it uses -n 4 to send 4 pings per IP.
For Linux/macOS, it uses -c 4 for the same purpose.
By default, the script sets the number of pings per IP to 4 and the timeout to 10 seconds for each server (These can be changed). This ensures consistent performance measurement across platforms.

This automation ensures that the DNS server configuration is not only efficient but also tailored to provide the fastest possible DNS resolution for the network.
