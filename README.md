# Types of DNS Record
## DNS Record
DNS records or zone files store information about domains. They consist of a series of text files written in the DNS syntax and are stored on DNS servers.
### Types of DNS record
- Start of Authority (SOA) record
- Host(A) record 
- Host AAAA record (quad A)
- CNAME record 
- Nameserver (NS) record 
- Mail exchange (MX) record
- PTR record
- TXT(text) record
- SRV record
- DCHID record
- DNAME record

### SOA record
SOA stands for "start of authority." It's an important DNS record type that stores admin information about a domain. This information includes the email address of the admin and when the domain was last updated.

### Host A Record (address)‍ 
Most commonly used to map a fully qualified domain name (FQDN) to an IPv4 address and acts as a translator by converting domain names to IP addresses.

### Host AAAA record
Similar to A Records but maps to an IPv6 address (smartphones prefer IPv6, if available).
Usage of the AAAA record for DNS resolution has great potential because it uses IPV6, which is an improvement over IPV4. Also, as the internet keeps growing and we're running out of IPV4 addresses, the potential for AAAA records is high.
AAAA records are used to resolve a domain name to the newer IPV6 protocol address.

### CNAME record
CNAME—or, in full, "canonical name"—is a DNS record that points a domain name (an alias) to another domain. In a CNAME record, the alias doesn't point to an IP address. And the domain name that the alias points to is the canonical name. For example, the subdomain ng.example.com can point to example.com using CNAME. Here example.com points to the actual IP address using an A record.
### NS record 
Specifies which name servers are authoritative for a domain or subdomains (these records should not be pointed to a CNAME).
A nameserver (NS) record specifies the authoritative DNS server for a domain. In other words, the NS record helps point to where internet applications like a web browser can find the IP address for a domain name.
### MX Record (Mail exchange)‍ 
Uses mail servers to map where to deliver email for a domain (should point to a mail server name and not to an IP address).
A mail exchange (MX) record, is a DNS record type that shows where emails for a domain should be routed to. In other words, an MX record makes it possible to direct emails to a mail server.
### PTR Record (pointer) 
A reverse of A and AAAA records, which maps IP addresses to domain names. These records require domain authority and can’t exist in the same zone as other DNS record types (put in reverse zones).
### TXT (text) Record‍ 
Allows administrators to add limited human and machine-readable notes and can be used for things such as email validation, site, and ownership verification, framework policies, etc., and doesn’t require specific formatting.Several services use this record to verify ownership of a domain.

### SRV record 
Using this DNS record type, it's possible to store the IP address and port for specific services.
 
### DCHID Record 
This DNS record type stores information related to dynamic host configuration protocol (DHCP).

### DNAME Record 
The full meaning of DNAME is "delegation name." This record type works very similarly to CNAME; however, it points all the subdomains for the alias to the canonical domain name.That is, pointing the DNAME for secondsite.com to example.com will also apply to staff.secondsite.com and any other subdomain.
