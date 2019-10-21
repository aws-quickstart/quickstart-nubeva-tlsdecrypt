# quickstart-nubeva-tlsdecrypt

This Quick Start adds five open source security & networking tools to your AWS Cloud environment. It deploys Moloch, ntopng, Wireshark, Zeek, and Suricata that provide advanced security visibility in your cloud. These tools are integrated with the Nubeva TOLS Decryption solution with provides deeper visibility into all TLS traffic, including TLS 1.2 w/PFS and TLS 1.3. You can choose to create a new VPC environment for your open source tools or deploy them into your existing VPC environment. After you deploy the Quick Start, you can add other AWS services, infrastructure components, and software layers to complete your test.

![Quick Start Nubeva TLS Decrypt Open Source Tool Architecture](https://nubevalabs.s3.amazonaws.com/quickstart.png )

Deployment steps:
1. Sign up for an AWS account at https://aws.amazon.com, select a region, and create a key pair.
2. Sign up for a Nubeva account at https://www.nubeva.com, deploy the tools from the launcher into your preferred region.
3. In the AWS CloudFormation console, select which tools to install.

Moloch Instructions:
1. Connect to the MolochELB on port 8005 using HTTP. Login in with the tooladmin username & password.
2. Point your Amazon VPC traffic mirroring sessions to the MolochELB Traffic Mirror Target (TMT)
3. For more instructions, see the [documentation](https://docs.nubeva.com/moloch)

Wireshark Instructions:
1. Connect to the Wireshark instance using SSH; ssh ubuntu@[ip.address]. Set the password for the ubuntu user: sudo passwd ubuntu
2. Connect to the WiresharkhELB on port 3389 using RDP. Login in with the ubuntu username & password from step 1
3. Point your Amazon VPC traffic mirroring sessions to the WiresharkELB Traffic Mirror Target (TMT)
4. For more instructions, see the [documentation](https://docs.nubeva.com/wireshark)

ntop Instructions:
1. Connect to the NtopELB on port 3000 using HTTP. Login in with the default username & password for ntop
2. Point your Amazon VPC traffic mirroring sessions to the ntopELB Traffic Mirror Target (TMT)
3. For more instructions, see the [documentation](https://docs.nubeva.com/ntop)

Zeek Instructions:
1. Connect to the Kibana link in the Zeek CTF Output section for access.
2. Point your Amazon VPC traffic mirroring sessions to the ZeekELB Traffic Mirror Target (TMT)
3. For more instructions, see the [documentation](https://docs.nubeva.com/zeek)

Suricata Instructions:
1. Connect to the Kibana link in the Suricata CTF Output section for access.
2. Point your Amazon VPC traffic mirroring sessions to the SuricataELB Traffic Mirror Target (TMT)
3. For more instructions, see the [documentation](https://docs.nubeva.com/suricata)
