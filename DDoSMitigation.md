# DDoS Mitigation

A threat faced by many independent journalists, news sites and bloggers is having their voices muted because their website is down or defaced. In many cases, this maybe an innocent and frustrating problem, but on occasion, it may be due to a 'denial of service' attack or a website takeover. This section of the Digital First Aid Kit will walk you through some basic steps to diagnose potential problems. If your site is under a denial of service attack, some immediate options for next steps are suggested.

In general, it is important to know that there are many reasons why your website can be down. Most often this is due to programming errors or technical problems at the company that hosts the site. Sometimes, other things like legal challenges can cause a host to turn a site off as well. Finding the problem and possible solutions to your website's problem can be cumbersome if you do not have hosting expertise. Therefore, when possible, the best first step is to contact a trusted person who can help with your website (your webmaster, the people who helped you set up your site, your internal staff if you have them and the company that hosts your site, or if none of these are available, [seek help from an organization you trust](SecureCommunication.md#seeking-and-providing-remote-help) ).

It is good practice to **contact your webmaster and the site host** after investigating these common challenges below! The problem you face may not have been reported on their status page, may be a temporary problem, or the site host may not yet be aware of the problem. A good relationship with your service providers goes a long way - be clear and polite and share the results of your investigation using these questions to help them quickly troubleshoot the problem.

## Start by answering some simple questions:

### Basic information

- Who built your website? Are they available to help?
- Who is your web hosting provider? This is the company that provides the server where your website lives. If you do not know, you can [use a tool](http://www.whoishostingthis.com/) to help.
- Do you have your account log in details for this hosting provider?
- Where did you purchase your domain name? In some cases this is also your website host, but it could also be another company.
- Do you have the log in details for the domain name service? If not, finding these is your first step to recovering your site
- Who else knows or may have access to these account details?


### Diagnostic information

There can be different reasons why your website is down. This can range from network to policy, hosting, blocking, software, defacement and performance problems. The section below explains what each of these problems is and how to diagnose which problem you are facing.

- **Is your web host working, but your website is unavailable?** 
    1. Check [on this website](http://www.isup.me/) 
        - Your site is up, but you can’t see it? 
            - This is a **network problem**. Your own internet connection could be having problems or be blocking your access to your site. 
            - This could also indicate that your account has been disabled: **Are you seeing a message from your web hosting provider?** 
                - You could have been taken offline for billing, legal, copyright or other reasons. 
                - This is a **policy problem**. First, make sure your billing information is up to date and that there is no outstanding balance on your hosting services or your domain name. If the message is due to a legal issue, [the resources provided](https://www.eff.org/issues/bloggers/legal/liability/IP) by EFF, while focused on US copyright laws, are a good place to learn more.
        - **Is your site not loading at all?** Your hosting company may be having problems, in which case you may be facing a **hosting problem**. 
            - Can you visit the website of your hosting company? Note that this is *not* the admin section of your own site, but that of the company or organization that hosts your site. Look or search for a 'status' blog (e.g. status.dreamhost.com); also search on twitter.com for other users discussing downtime at the host 
                - a simple search like '(company name) down' can often reveal whether others are having the same problem.
    2. **Can you visit other sites with similar content to your site?** 
        - Try visiting websites related to yours or covering similar issues. Also try using [Tor](https://www.torproject.org/projects/gettor.html) or [Psiphon](https://psiphon.ca/products.php) to access your site. If this helps, you have a **blocking problem** - you are still online for other parts of the world, but are being censored in your own country.
    3. **Are you seeing error messages?** 
        - This could be a **software problem**. You should reflect on any recent changes you or your team may have made and contact your webmaster. 
            - Sending your webmaster a screenshot, the link of the page you are having problems with and any error messages you see will help them figure out what might be causing the problem. 
            - You might also copy the error messages into a search to see if they are easily fixed.
    4. **Are you seeing a website that is not yours? Are you receiving a warning from your browser about malware on your own site?** 
        - This could be a **defacement problem**. See below for next steps; you will need to work with your web hosting provider and review the Account Hijacking section.
    5. **Is your site loading intermittently or unusually slowly?** 
        - Your site may be overwhelmed by the number and speed of requests for pages it is receiving - this is a **performance problem**. This could be 'good' insofar as your site has become more popular and it simply needs some improvements to respond to more readers. 
            - check your site analytics for a long-term pattern in growth. 
            - Contact your webmaster or hosting provider for guidance. Many popular blogging and CMS platforms (Joomla, Wordpress, Drupal and others) have plugins to help cache your website locally and integrate CDNs, which can dramatically improve site performance and resilience. Many of the solutions below can also help performance problems.

## First steps to mitigate the problem:

### When you are suffering from a Denial of Service attack

If the above diagnoses do not help (or you are experiencing a severe **performance problem**, your site may be the victim of a **'denial of service' attack**, where a malicious user (or users), try to view the website repeatedly and rapidly (using automated tools), and in doing so crowd out legitimate readers. Sometimes it’s one 'attacker' trying to do this to your site, which doesn’t usually cause much of a problem - unless you pay for bandwidth. More common is the 'Distributed' denial of Service (DDoS), where an attacker uses thousands of machines under his control to targets a site.

- Step 1: Contact a trusted person who can help with your website (your webmaster, the people who helped you set up your site, your internal staff if you have them and the company that hosts your site).
- Step 2: Work with the company you bought your domain from (like EasyDNS, [Network Solutions](http://www.networksolutions.com/support/how-to-manage-advanced-dns-records/), [GoDaddy](http://support.godaddy.com/help/article/680/managing-dns-for-your-domain-names)) and change the 'Time to Live' or TTL to 1 hour. This can help you redirect your site much faster once it comes under attack (the default is 72 hours, or three days). This setting will often be found in 'advanced' properties for your domain, sometimes part of the SRV or Service records.
- Step 3: Move your site to a DDoS mitigation service [full list](https://github.com/OpenInternet/MyWebsiteIsDown/blob/master/MyWebsiteIsDown.md#mitigation-services). To start:
    - [Deflect.ca](https://deflect.ca/)
    - [Google's Project Shield](https://projectshield.withgoogle.com/en/)
    - [CloudFlare's Project Galileo](https://www.cloudflare.com/galileo)
- Step 4: As soon as you have regained control, review your needs and decide between a secure hosting provider or simply continuing with your DDoS mitigation service.

### When you are suffering from a Website Defacement

- Step 1: Verify that this is a malicious takeover of your website. An unfortunate but legal practice is to buy recently expired domain names to 'take over' the traffic they had for advertising purposes. It is very important to keep payments for your domain name in order.
- Step 2: If your website has been defaced, first regain control of your website login account and reset its password, see the Account Hijacking section for help.
- Step 3: Make a backup of the defaced site that can later be used for investigation of the defacement.
- Step 4: Temporarily turn off your website - use a simple landing page or 'parked' page.
- Step 5: Determine how your site was hacked. Your hosting provider may be able to help. Common problems are older parts of your site with custom scripts/tools running on them, out of date content management systems, and custom programming with security flaws.
- Step 6: Restore your original from backups. If neither you, nor your hosting company have backups, you may have to re-build your website from scratch! Also note that if your only backups are at your hosting provider, an attacker may be able to delete those when they take control of your site!
- Step 7: Move to a DDoS Mitigtion service or secure hosting provider. Deflect.ca can support you in protecting your site from online attacks. CloudFlare can also block many common attacks. Secure hosting providers such as VirtualRoad/Qurium go to great lengths to detect and prevent such attacks.


## Don't stop here! Important next steps

**Don’t wait until you have been attacked!** All of the services listed below will work quickly to help you recover during or after an attack, but you can protect yourself now, before any attack happens! This can reduce costs by lowering your bandwidth usage and keeping you online during an attack. Once you’ve been hit, it can take up to three days for the internet to 'find' you at your new, protected address - so in almost every case, it’s much better to **be prepared and get started now**.

1. **Secure Hosting Providers** require you to move your website completely to their servers - you’re changing hosting providers. Many of them can help you through this. The benefits of this include the hosted solution often providing many other protection features in addition to DDoS mitigation; the downside can be cost (depending on what you currently pay) and  control - you need to be able to trust your domain host, as they have a lot of control over your website.
    - Pros:
        - Provides one central service for most, if not all, your website needs
        - Provides protection services for DDoS, hacking and spam attacks
        - Often includes many secondary services and consulting, and even limited legal defense in some cases
        - Full support teams are often on staff to help
    - Cons:
        - You must host your website with the service
        - You must trust the service to manage your site and defend your rights
        - These services are often much more expensive (but you don’t have to pay other hosting / DNS services anymore!)

2. **DDoS Mitigation services** let you continue hosting your site wherever it is, and just change how others on the internet find and access it - this is generally much easier to set up. These services have servers around the world that, essentially, get out in front of your website and absorb or ignore malicious traffic. They 'mirror' and serve constantly-updated copies of your site. These services are easy to set up and you maintain complete control of your website and hosting setup. One challenge with proxied services is that very complex websites can sometimes experience problems with non-admin user logins and complex interactive/javascript area. Please discuss these with your webmaster and the proxy service as most can be resolved.
    - Pros:
        - Lower cost (often with a free level)
        - Quick and easy to set up
        - You don’t have to change your existing website host
        - You can change or quit the service at any time
    - Cons:
        - Fewer support options
        - Focused primarily on just mitigating DDoS attacks - does not necessarily include help with malware or spammers.
        - SSL (encrypted) traffic will be briefly decrypted and re-encrypted by the proxy server to pass it from their proxy to your server.

3. Choose a specific provider - for any service, you must be comfortable with the provider. This relates to trust, but also understanding their business model: Is it fee-for-service? If there’s a free version, does it receive less support than a paid alternative? Is it funded by governments? It is best to cover as much detail up front as possible to avoid surprises down the road.

### For all services ask yourself the following questions:

- How is the company/organization structured and sustained? What types of vetting or reporting are they required to do, if any?
- Consider what country/countries they have a legal presence in and which they would be required to comply with law enforcement and other legal requests
- What logs are created, and for how long are they available?
- Are there restrictions regarding the type of content the service will host/proxy, and could they have an impact on your site?
- Are there restrictions on the countries where they can provide service?
- Do they accept a form of payment you can use? Can you afford their service?
- Secure communications - you should be able to log in securely and communicate with the service provider privately.
- Is there an option for two-factor authentication, to improve the security of administrator access? This or related secure access policies can help reduce the threat of other forms of attacks against your website.
- What type of ongoing support will you have access to? Is there an additional cost for support, and/or will you receive sufficient support if you are using a 'free' tier?
- Can you 'test-drive' your website before you move over via a staging site?

### Questions for secure hosting services

- Do they offer full support in moving your site over to their service?
- Are the services equal to or better than your current host, at least for the tools/services you use? Top things to check are:
    - Management dashboards like cPanel
    - Email accounts (how many, quotas, access via SMTP, IMAP)
    - Databases (how many, types, access)
    - Remote access via SFTP/SSH
    - Support for the programming language (PHP, Perl, Ruby, cgi-bin access...) or CMS (Drupal, Joomla, Wordpress…) that your site uses

### Questions for DDoS Mitigation services:

- If you use SSL (also known as HTTPS or secure web traffic), ask how they manage SSL. In some configurations, it may be easiest to share your private SSL key. If you do so, you need to have a high level of trust in the service provider, as they can 'impersonate' your site (indeed, this is what you are asking them to do by providing a proxy!)
- Ask about how administration /editorial logins and pages are managed
- Talk about any interactive parts of your website (users who log in, comment, admin/editorial needs, complex interactive pages/javascript/animations) - different proxy services manage these differently; you will need to test these before switching completely.

### Specific Mitigation Services

Specific services are [listed with extensive notes](https://github.com/OpenInternet/MyWebsiteIsDown/blob/master/MyWebsiteIsDown.md#mitigation-service). Please note that the list provided is not a complete listing of services; there are many more. However, these services all represent good starting points, as they have been used by other members in the independent media / human rights / free speech communities. For immediate coverage, here are options:

- Secure Hosting Services:
    - [Qurium (formerly Virtual Road)](https://www.qurium.org/)
    - [The Positive Internet Company](http://www.positive-internet.com/services/vip-hosting)
    - [Greenhost](https://greenhost.net/)

- DDoS Mitigation Services:
    - [Deflect.ca](https://deflect.ca/)
    - [Google's Project Shield](https://projectshield.withgoogle.com/en/)
    - [CloudFlare's Project Galileo](https://www.cloudflare.com/galileo)

## Take extra precaution against attackers

Even if you have not experienced a Denial of Service attack, this guide offers steps to prepare for one, hopefully preventing any downtime at all. Go straight to the [Responding to a Denial of Service Attack](https://github.com/OpenInternet/MyWebsiteIsDown/blob/master/MyWebsiteIsDown.md#responding-to-a-denial-of-service-attack) section to investigate common solutions you can implement now, before being attacked. At the Helpful Resource section you can find guides to keep your site alive.

- **Backups**: It’s always good to ensure you have backups (that you store somewhere other than the same place your website is!). Many hosts and website platforms include this as part of their service, but it’s best to also have additional, offline copies.
- **Keep up to date**: If you are using a Content Management System (CMS) such as WordPress or Drupal, check to make sure that your website technology is updated to the latest software, especially if  there have been security updates. If you are using custom software, consider moving to a CMS that receives regular updates.
- **Monitoring**: There are many services that can constantly check on your site and email or text you if it goes down. [This Mashable article](http://mashable.com/2010/04/09/free-uptime-monitoring/) lists ten popular ones. Be aware that the email or phone number you use for monitoring will be clearly associated with managing the website.

## Investigate

If you have been the victim of a **'Denial of Service'** or **Defacement attack**, it can be valuable to understand why you've been attacked and why now.

**Why you've been attacked and why now**: Who do you think might be interested in targeting your website or your organization? Have you recently posted something controversial, could this threat be related to your work or does your website receive a lot of traffic and did your domain name expire? Why now? Could a recent change to your website have made you a target for Denial of Service attacks or Defacement attacks? In the section on helpful resources there are links to guides that give you tips and tricks on how to prevent digital emergencies and be proactive in your digital security.

## Helpful resources:

- [My Website is Down](https://github.com/OpenInternet/MyWebsiteIsDown)
- [Keep your site alive](https://www.eff.org/keeping-your-site-alive)
- [Security in a Box](https://securityinabox.org/en/chapter_7_2)
- [Threat modeling, Surveillance Self Defense Guide](https://ssd.eff.org/risk/threats)

