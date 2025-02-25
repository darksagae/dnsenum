# dnsenum
`dnsenum` is a powerful tool used for DNS enumeration and gathering information about domains. Below are some common commands and examples of how to use `dnsenum` on Kali Linux.

### Basic Command Syntax

```bash
dnsenum [options] <domain>
```

### Common Options

- `-h`: Display help information.
- `-s`: Specify a specific DNS server to query.
- `-f`: Use a specific file for subdomain enumeration.
- `-r`: Perform reverse lookup.
- `-o`: Specify an output file to save results.
- `-q`: Quiet mode, less verbose output.

### Examples

1. **Basic DNS Enumeration**

   To perform a basic DNS enumeration on a domain:

   ```bash
   dnsenum example.com
   ```

2. **Using a Specific DNS Server**

   To query a specific DNS server:

   ```bash
   dnsenum -s 8.8.8.8 example.com
   ```

3. **Saving Output to a File**

   To save the results to a file:

   ```bash
   dnsenum -o output.txt example.com
   ```

4. **Performing Reverse Lookup**

   To perform a reverse lookup for a specific IP address:

   ```bash
   dnsenum -r 192.168.1.1
   ```

5. **Using a Subdomain File**

   To use a custom subdomain enumeration file:

   ```bash
   dnsenum -f subdomains.txt example.com
   ```

6. **Quiet Mode**

   To run `dnsenum` in quiet mode:

   ```bash
   dnsenum -q example.com
   ```

### Conclusion

These commands should help you get started with DNS enumeration using `dnsenum` on Kali Linux. Make sure to replace `example.com` with the actual domain you want to enumerate. Always ensure you have permission to perform such activities on the target domain to comply with ethical hacking practices.


                                                        ALTERNATIVE
`dnsenum` is a powerful tool available in Kali Linux for enumerating DNS information about a domain. It is particularly useful for gathering details such as name servers, IP addresses, and other DNS records. Below are some common commands and examples of how to use `dnsenum`.

### Basic Usage

To run `dnsenum`, you can use the following command structure:

```bash
dnsenum [options] <domain>
```

### Common Commands and Examples

1. **Basic Enumeration**:
   To perform a basic enumeration of a domain, simply run:
   ```bash
   dnsenum example.com
   ```
   This command will gather standard DNS records for the specified domain.

2. **Brute Force Subdomains**:
   To brute force subdomains using a wordlist, you can use:
   ```bash
   dnsenum --enum --dnsserver <dns_server> --f <wordlist.txt> example.com
   ```
   Replace `<dns_server>` with the DNS server you want to query and `<wordlist.txt>` with the path to your wordlist file.

3. **Reverse Lookup**:
   To perform a reverse lookup on a specific IP address range, use:
   ```bash
   dnsenum --reverse <IP_range>
   ```
   This will help you find associated domain names for the given IP range.

4. **Save Output to File**:
   To save the output of your enumeration to a file, you can use:
   ```bash
   dnsenum --output <filename> example.com
   ```
   This command will save the results to the specified file.

5. **Verbose Mode**:
   For more detailed output, you can enable verbose mode:
   ```bash
   dnsenum --verbose example.com
   ```
   This will provide additional information during the enumeration process.

### Additional Options

- **--help**: Display help information about `dnsenum` and its options.
- **--enum**: Perform a full enumeration of the domain.
- **--dnsserver**: Specify a DNS server to use for queries.
- **--f**: Specify a file containing a list of subdomains for brute forcing.

These commands allow you to effectively gather DNS information and perform reconnaissance on a target domain using `dnsenum` in Kali Linux.

---
Learn more:
1. [dnsrecon | Kali Linux Tools](https://www.kali.org/tools/dnsrecon/)
2. [How to Use DNS Analysis Tools in Kali Linux | Cybrary](https://www.cybrary.it/blog/use-dns-analysis-tools-kali-linux)
3. [dnschef | Kali Linux Tools](https://www.kali.org/tools/dnschef/)




                                                  ALTERNATIVE
