# Awesome Password Cracking  [![Awesome](https://awesome.re/badge.svg)](https://awesome.re) with stars

In cryptanalysis and computer security, password cracking is the process of recovering passwords from data that has been stored in or transmitted by a computer system in scrambled form. A common approach ([brute-force attack](https://en.wikipedia.org/wiki/Brute-force_attack)) is to repeatedly try guesses for the password and to check them against an available cryptographic hash of the password.

This is a curated list of awesome tools, research, papers and other projects related to password cracking and password security by [@n0kovo@infosec.exchange](https://infosec.exchange/@n0kovo/?l).

Read [CONTRIBUTING.md](https://github.com/narkopolo/awesome-password-cracking/blob/main/CONTRIBUTING.md) ⭐ 913 | 🐛 0 | 📅 2026-03-15 before contributing! In short:

* If you think an item shouldn't be here [open an issue](https://github.com/narkopolo/awesome-password-cracking/issues/new) ⭐ 913 | 🐛 0 | 📅 2026-03-15
* If in doubt, use [awesome-lint](https://github.com/sindresorhus/awesome-lint) ⭐ 749 | 🐛 3 | 🌐 JavaScript | 📅 2026-01-30
* List is alphabetically sorted

## Contents

* [Awesome Password Cracking  ](#awesome-password-cracking--)
  * [Contents](#contents)
  * [Books](#books)
  * [Cloud](#cloud)
  * [Conversion](#conversion)
  * [Hashcat](#hashcat)
    * [Automation](#automation)
    * [Distributed cracking](#distributed-cracking)
    * [Rules](#rules)
    * [Rule tools](#rule-tools)
    * [Web interfaces](#web-interfaces)
  * [John the Ripper](#john-the-ripper)
  * [Misc](#misc)
    * [Notable People](#notable-people)
  * [Websites](#websites)
    * [Communities](#communities)
    * [Lookup services](#lookup-services)
  * [Wordlist tools](#wordlist-tools)
    * [Analysis](#analysis)
    * [Generation/Manipulation](#generationmanipulation)
  * [Wordlists](#wordlists)
    * [Laguage specific](#laguage-specific)
    * [Other](#other)
  * [Specific file formats](#specific-file-formats)
    * [PDF](#pdf)
    * [JKS](#jks)
    * [ZIP](#zip)
  * [Machine Learning / AI](#machine-learning--ai)
  * [Research](#research)
    * [Articles and Blog Posts](#articles-and-blog-posts)
    * [Papers](#papers)
    * [Talks](#talks)

## Books

* [Hash Crack: Password Cracking Manual (v3)](https://www.amazon.com/-/en/Joshua-Picolet/dp/1793458618) - Password Cracking Manual v3 is an expanded reference guide for password recovery (cracking) methods, tools, and analysis techniques.

## Cloud

* [Penglab](https://github.com/mxrch/penglab) ⭐ 969 | 🐛 10 | 🌐 Jupyter Notebook | 📅 2023-07-17 - Abuse of Google Colab for cracking hashes.
* [NPK](https://github.com/c6fc/npk) ⭐ 653 | 🐛 15 | 🌐 JavaScript | 📅 2025-12-13 - NPK is a distributed hash-cracking platform built entirely of serverless components in AWS including Cognito, DynamoDB, and S3.
* [Cloudtopolis](https://github.com/JoelGMSec/Cloudtopolis) ⭐ 417 | 🐛 2 | 🌐 PowerShell | 📅 2024-08-22 - A tool that facilitates the installation and provisioning of Hashtopolis on the Google Cloud Shell platform, quickly and completely unattended (and also, free!).
* [Rook](https://github.com/JumpsecLabs/Rook) ⭐ 85 | 🐛 1 | 🌐 Python | 📅 2019-11-13 - Automates the creation of AWS p3 instances for use in GPU-based password cracking.
* [Cloud\_crack](https://github.com/lordsaibat/Cloud_crack) ⭐ 43 | 🐛 0 | 🌐 HCL | 📅 2019-03-20 - Crack passwords using Terraform and AWS.
* [Cloudcat](https://github.com/stormfleet/cloudcat) ⭐ 15 | 🐛 1 | 🌐 Python | 📅 2019-09-04 - A script to automate the creation of cloud infrastructure for hash cracking.
* [Cloudstomp](https://github.com/Fmstrat/cloudstomp) ⭐ 3 | 🐛 0 | 🌐 Python | 📅 2019-01-18 - Automated deployment of instances on EC2 via plugin for high CPU/GPU applications at the lowest price.

## Conversion

* [hcxtools](https://github.com/ZerBea/hcxtools) ⭐ 2,359 | 🐛 1 | 🌐 C | 📅 2026-04-02 - Portable solution for conversion of cap/pcap/pcapng (gz compressed) WiFi dump files to hashcat formats.
* [7z2hashcat](https://github.com/philsmd/7z2hashcat) ⭐ 423 | 🐛 5 | 🌐 Perl | 📅 2024-06-15 - Extract information from password-protected .7z archives (and .sfx files) such that you can crack these "hashes" with hashcat.
* [itunes\_backup2hashcat](https://github.com/philsmd/itunes_backup2hashcat) ⭐ 117 | 🐛 0 | 🌐 Perl | 📅 2017-02-04 - Extract the information needed from the Manifest.plist files to convert it to hashes compatible with hashcat.
* [WINHELLO2hashcat](https://github.com/Banaanhangwagen/WINHELLO2hashcat) ⭐ 84 | 🐛 1 | 🌐 Python | 📅 2022-04-22 - With this tool one can extract the "hash" from a WINDOWS HELLO PIN. This hash can be cracked with Hashcat.
* [MacinHash](https://github.com/jmagers/MacinHash) ⭐ 37 | 🐛 0 | 🌐 Python | 📅 2018-12-03 - Convert macOS plist password file to hash file for password crackers.
* [NetNTLM-Hashcat](https://github.com/ins1gn1a/NetNTLM-Hashcat) ⭐ 35 | 🐛 0 | 🌐 Python | 📅 2019-11-24 - Converts John The Ripper/Cain format hashes (singular, or in bulk) to HashCat compatible hash format.
* [bitwarden2hashcat](https://github.com/0x6470/bitwarden2hashcat) ⭐ 25 | 🐛 2 | 🌐 Python | 📅 2022-03-17 - A tool that converts Bitwarden's data into a hashcat-suitable hash.
* [Rubeus-to-Hashcat](https://github.com/PwnDexter/Rubeus-to-Hashcat) ⭐ 11 | 🐛 0 | 🌐 Python | 📅 2020-01-16 - Converts / formats Rubeus kerberoasting output into hashcat readable format.
* [hc\_to\_7z](https://github.com/philsmd/hc_to_7z) ⭐ 8 | 🐛 0 | 🌐 Perl | 📅 2024-05-07 - Convert 7-Zip hashcat hashes back to 7z archives.
* [mongodb2hashcat](https://github.com/philsmd/mongodb2hashcat) ⭐ 7 | 🐛 3 | 🌐 JavaScript | 📅 2020-10-11 - Extract hashes from the MongoDB database server to a hash format that hashcat accepts: -m 24100 (SCRAM-SHA-1) or -m 24200 (SCRAM-SHA-256).

## Hashcat

*[Hashcat](https://github.com/hashcat/hashcat) ⭐ 25,740 | 🐛 326 | 🌐 C | 📅 2026-02-20 is the "World's fastest and most advanced password recovery utility." The following are projects directly related to Hashcat in one way or another.*

* [hashcat-utils](https://github.com/hashcat/hashcat-utils/) ⭐ 1,565 | 🐛 21 | 🌐 C | 📅 2025-11-08 - Small utilities that are useful in advanced password cracking.
* [known\_hosts-hashcat](https://github.com/chris408/known_hosts-hashcat) ⭐ 339 | 🐛 3 | 🌐 Python | 📅 2024-01-03 - A guide and tool for cracking ssh known\_hosts files with hashcat.
* [docker-hashcat](https://github.com/dizcza/docker-hashcat) ⭐ 159 | 🐛 2 | 🌐 Dockerfile | 📅 2025-08-19 - Latest hashcat docker for Ubuntu 18.04 CUDA, OpenCL, and POCL.
* [Hashcat-Stuffs](https://github.com/xfox64x/Hashcat-Stuffs) ⭐ 50 | 🐛 0 | 🌐 PowerShell | 📅 2019-12-18 - Collection of hashcat lists and things.
* [Autocrack](https://github.com/pry0cc/autocrack) ⭐ 41 | 🐛 3 | 🌐 Shell | 📅 2023-03-16 - A set of client and server tools for automatically, and lightly automatically cracking hashes.
* [pyhashcat](https://github.com/f0cker/pyhashcat) ⭐ 33 | 🐛 0 | 🌐 C | 📅 2021-06-11 - Python C API binding to libhashcat.
* [Hashfilter](https://github.com/bharshbarger/Hashfilter) - Read a hashcat potfile and parse different types into a sqlite database.

### Automation

* [hate\_crack](https://github.com/trustedsec/hate_crack) ⭐ 1,817 | 🐛 1 | 🌐 Python | 📅 2026-04-08 - A tool for automating cracking methodologies through Hashcat from the TrustedSec team.
* [Naive hashcat](https://github.com/brannondorsey/naive-hashcat) ⭐ 1,389 | 🐛 11 | 🌐 C | 📅 2022-01-10 - Naive hashcat is a plug-and-play script that is pre-configured with naive, emperically-tested, "good enough" parameters/attack types.
* [hat](https://github.com/sp00ks-git/hat) ⭐ 306 | 🐛 1 | 🌐 Python | 📅 2024-06-14 - An Automated Hashcat Tool for common wordlists and rules to speed up the process of cracking hashes during engagements.
* [autocrack](https://github.com/timbo05sec/autocrack) ⭐ 120 | 🐛 0 | 🌐 Python | 📅 2018-04-16 - Hashcat wrapper to help automate the cracking process.

### Distributed cracking

* [Hashtopolis](https://github.com/hashtopolis/server) ⭐ 1,735 | 🐛 229 | 🌐 PHP | 📅 2026-04-10 - A multi-platform client-server tool for distributing hashcat tasks to multiple computers.
* [CrackLord](https://github.com/jmmcatee/cracklord) ⭐ 392 | 🐛 34 | 🌐 Go | 📅 2022-09-22 - Queue and resource system for cracking passwords.
* [Kraken](https://github.com/arcaneiceman/kraken) ⭐ 327 | 🐛 9 | 🌐 JavaScript | 📅 2023-06-02 - A multi-platform distributed brute-force password cracking system.
* [fitcrack](https://github.com/nesfit/fitcrack) ⭐ 172 | 🐛 27 | 🌐 C | 📅 2026-04-09 - A hashcat-based distributed password cracking system.
* [Hashstation](https://github.com/hashstation/hashstation) ⭐ 10 | 🐛 3 | 🌐 C | 📅 2024-01-19 - Hashstation is a BOINC-based distributed password cracking system with a built-in web interface.

### Rules

* [OneRuleToRuleThemAll](https://github.com/NotSoSecure/password_cracking_rules) ⭐ 1,613 | 🐛 6 | 📅 2021-12-09 - "One rule to crack all passwords. or atleast we hope so."
* [Hob0Rules](https://github.com/praetorian-inc/Hob0Rules) ⚠️ Archived - Password cracking rules for Hashcat based on statistics and industry patterns.
* [Kaonashi](https://github.com/kaonashi-passwords/Kaonashi) ⭐ 1,088 | 🐛 1 | 📅 2022-04-22 - Wordlist, rules and masks from Kaonashi project (RootedCON 2019).
* [OneRuleToRuleThemStill](https://github.com/stealthsploit/OneRuleToRuleThemStill) ⭐ 626 | 🐛 0 | 📅 2024-10-16 - "A revamped and updated version of my original OneRuleToRuleThemAll hashcat rule."
* [nsa-rules](https://github.com/NSAKEY/nsa-rules) ⭐ 562 | 🐛 0 | 🌐 Shell | 📅 2017-01-03 - Password cracking rules and masks for hashcat generated from cracked passwords.
* [clem9669 rules](https://github.com/clem9669/hashcat-rule) ⭐ 463 | 🐛 0 | 📅 2024-09-02 - Rule for hashcat or john.
* [pantagrule](https://github.com/rarecoil/pantagrule) ⭐ 398 | 🐛 0 | 📅 2020-11-26 - Large hashcat rulesets generated from real-world compromised passwords.
* [hashcat rules collection](https://github.com/narkopolo/hashcat-rules-collection) ⭐ 150 | 🐛 0 | 📅 2026-01-16 - Probably the largest collection of hashcat rules out there.
* [nyxgeek-rules](https://github.com/nyxgeek/nyxgeek-rules) ⭐ 94 | 🐛 0 | 🌐 Shell | 📅 2024-08-19 - Custom password cracking rules for Hashcat and John the Ripper.

### Rule tools

* [duprule](https://github.com/mhasbini/duprule) ⭐ 48 | 🐛 4 | 🌐 Rust | 📅 2025-01-14 - Detect & filter duplicate hashcat rules.
* [ruleprocessorY](https://github.com/TheWorkingDeveloper/ruleprocessorY) ⭐ 37 | 🐛 4 | 🌐 C++ | 📅 2025-11-25 - A next-gen Rule processor with complex multibyte character support built to support Hashcat.

### Web interfaces

* [CrackQ](https://github.com/f0cker/crackq) ⭐ 939 | 🐛 10 | 🌐 Python | 📅 2024-09-03 - A Python Hashcat cracking queue system.
* [Hashview](https://github.com/hashview/hashview) ⭐ 388 | 🐛 61 | 🌐 Python | 📅 2026-02-17 - A web front-end for password cracking and analytics.
* [crackerjack](https://github.com/ctxis/crackerjack) ⭐ 380 | 🐛 8 | 🌐 Python | 📅 2024-02-01 - CrackerJack is a Web GUI for Hashcat developed in Python.
* [WebHashCat](https://github.com/hegusung/WebHashcat) ⭐ 321 | 🐛 13 | 🌐 JavaScript | 📅 2026-04-04 - WebHashcat is a very simple but efficient web interface for hashcat password cracking tool.
* [Wavecrack](https://github.com/wavestone-cdt/wavecrack) ⭐ 170 | 🐛 1 | 🌐 Python | 📅 2021-09-09 - Wavestone's web interface for password cracking with hashcat.
* [hashpass](https://github.com/dj-zombie/hashpass) ⭐ 47 | 🐛 2 | 🌐 Vue | 📅 2022-07-20 - Hash cracking WebApp & Server for hashcat.

## John the Ripper

*[John the Ripper](https://github.com/openwall/john) ⭐ 12,970 | 🐛 492 | 🌐 C | 📅 2026-04-09 is "an Open Source password security auditing and password recovery tool available for many operating systems." The following are projects directly related to John the Ripper in one way or another.*

* [BitCracker](https://github.com/e-ago/bitcracker) ⭐ 946 | 🐛 57 | 🌐 C | 📅 2024-05-31 - BitCracker is the first open source password cracking tool for memory units encrypted with BitLocker.
* [johnny](https://github.com/openwall/johnny) ⭐ 625 | 🐛 20 | 🌐 C++ | 📅 2023-09-29 - GUI frontend to John the Ripper.

## Misc

* [Name That Hash](https://github.com/HashPals/Name-That-Hash) ⭐ 1,642 | 🐛 7 | 🌐 Python | 📅 2025-12-19 - Don't know what type of hash it is? Name That Hash will name that hash type! Identify MD5, SHA256 and 300+ other hashes. Comes with a neat web app.
* [hashgen](https://github.com/cyclone-github/hashgen) ⭐ 39 | 🐛 0 | 🌐 Go | 📅 2026-04-11 - Hashgen is a simple yet very fast CLI hash generator written in Go and cross compiled for Linux, Windows & Mac.
* [Hashes](https://github.com/zefr0x/hashes) ⭐ 31 | 🐛 1 | 🌐 Python | 📅 2025-05-23 - Identify hashing algorithms (GUI frontend for Name That Hash).

### Notable People

* Alotdv - [Twitter](https://twitter.com/AlongExc).
* Clem9669 - [GitHub](https://github.com/clem9669).
* Coolbry95 - [GitHub](https://github.com/coolbry95) / [Twitter](https://twitter.com/coolbry95).
* Dakykilla - [GitHub](https://github.com/dakykilla) / [Twitter](https://twitter.com/dakykilla).
* Dropdeadfu - [GitHub](https://github.com/dropdeadfu) / [Twitter](https://twitter.com/dropdeadfu).
* Epixoip - [GitHub](https://github.com/epixoip) / [Mastodon](https://infosec.exchange/@epixoip) / [Twitter](https://twitter.com/jmgosney).
* Evilmog - [GitHub](https://github.com/evilmog/) / [Mastodon](https://infosec.exchange/@evilmog) / [Twitter](https://twitter.com/Evil_Mog).
* Hydraze - [GitHub](https://github.com/Hydraze) / [Mastodon](https://infosec.exchange/@hydraze) / [Twitter](https://twitter.com/Hydraze).
* JakeWnuk - [GitHub](https://github.com/jakewnuk).
* Kontrast23 - [GitHub](https://github.com/kontrast23) / [Twitter](https://twitter.com/marco_preuss).
* M3g9tr0n - [GitHub](https://github.com/m3g9tr0n) / [Twitter](https://twitter.com/m3g9tr0n).
* Matrix - [GitHub](https://github.com/matrix) / [Twitter](https://twitter.com/gm4tr1x).
* Minga - [Twitter](https://twitter.com/mingadotcom).
* N0kovo - [GitHub](https://github.com/n0kovo) / [Mastodon](https://infosec.exchange/@n0kovo) / [Twitter](https://twitter.com/n0kovos).
* NSAKEY - [GitHub](https://github.com/NSAKEY) / [Twitter](https://twitter.com/_NSAKEY) / [Website](https://abigisp.com/).
* NullMode - [GitHub](https://github.com/NullMode) / [Mastodon](https://infosec.exchange/@nullmode_@twtr.plus) / [Twitter](https://twitter.com/nullmode_).
* Paule965 - [Twitter](https://twitter.com/paule965).
* Philsmd - [GitHub](https://github.com/philsmd) / [Twitter](https://twitter.com/philsmd).
* Roycewilliams - [GitHub](https://github.com/roycewilliams) / [Mastodon](https://infosec.exchange/@tychotithonus) / [Twitter](https://twitter.com/TychoTithonus).
* RuraPenthe - [GitHub](https://github.com/bitcrackcyber) / [Mastodon](https://infosec.exchange/@rurapenthe) / [Twitter](https://twitter.com/RuraPenthe0).
* S3in!c - [GitHub](https://github.com/s3inlc) / [Mastodon](https://infosec.exchange/@s3inlc) / [Twitter](https://twitter.com/s3inlc).
* Tehnlulz - [GitHub](https://github.com/tehnlulz) / [Twitter](https://twitter.com/tehnlulz).
* The\_Mechanic - [GitHub](https://github.com/th3mechanic) / [Twitter](https://twitter.com/th3_m3chan1c).
* ToXiC - [Twitter](https://twitter.com/yiannistox).
* Undeath - [GitHub](https://github.com/undeath).
* Unix-ninja - [GitHub](https://github.com/unix-ninja) / [Mastodon](https://infosec.exchange/@unix_ninja@twitterbridge.jannis.rocks) / [Twitter](https://twitter.com/unix_ninja).
* Xan - [GitHub](https://github.com/Xanadrel) / [Mastodon](https://infosec.exchange/@Xanadrel) / [Twitter](https://twitter.com/Xanadrel).

## Websites

### Communities

* [hashcat Forum](https://hashcat.net/forum/) - Forum by the developers of hashcat.
* [Hashmob](https://hashmob.net/) - A growing password recovery community aimed towards being a center point of collaboration for cryptography enthusiasts. Huge wordlist collection and a lookup service too.
* [Hashkiller Forum](https://forum.hashkiller.io/) - A password cracking forum with over 20,000 registered users.

### Lookup services

* [CMD5](https://www.cmd5.org/) - Provides online MD5 / sha1/ mysql / sha256 encryption and decryption services.
* [CrackStation](https://crackstation.net/) - Free hash lookup service supplying wordlists as well.
* [gohashmob](https://github.com/n0kovo/gohashmob) ⭐ 14 | 🐛 0 | 🌐 Go | 📅 2023-04-16 - Go CLI app to quickly lookup hashes using the HashMob API.
* [Hashes.com](https://hashes.com/) - A hash lookup service with paid features.
* [Hashkiller](https://hashkiller.io/) - A hash lookup service with a forum.
* [Online Hash Crack](https://www.onlinehashcrack.com/) - Cloud password recovery service.

## Wordlist tools

*Tools for analyzing, generating and manipulating wordlists.*

### Analysis

* [PACK](https://github.com/iphelix/pack) ⭐ 873 | 🐛 9 | 🌐 Python | 📅 2019-12-10 - A collection of utilities developed to aid in analysis of password lists in order to enhance password cracking through pattern detection of masks, rules, character-sets and other password characteristics.
* [Pipal](https://github.com/digininja/pipal) ⭐ 662 | 🐛 8 | 🌐 Ruby | 📅 2023-08-27 - THE password analyser.
* [pcfg\_cracker](https://github.com/lakiw/pcfg_cracker) ⭐ 369 | 🐛 12 | 🌐 Python | 📅 2025-09-02 - This project uses machine learning to identify password creation habits of users.
* [Graphcat](https://github.com/Orange-Cyberdefense/graphcat) ⭐ 164 | 🐛 3 | 🌐 Python | 📅 2023-02-17 - Generate graphs and charts based on password cracking result.
* [password-stretcher](https://github.com/thetechromancer/password-stretcher) ⭐ 39 | 🐛 2 | 🌐 Python | 📅 2022-12-08 - Generate "disgusting quantities" of passwords from websites, files, or stdin. Compliments password-smelter.
* [password-smelter](https://github.com/TheTechromancer/password-smelter) ⭐ 21 | 🐛 0 | 🌐 Python | 📅 2024-01-17 - Ingests passwords from hashcat, etc. and outputs to HTML, Markdown, XLSX, PNG, JSON. Dark and light themes supported. Compliments password-stretcher.

### Generation/Manipulation

* [CUPP](https://github.com/Mebus/cupp) ⭐ 5,858 | 🐛 48 | 🌐 Python | 📅 2025-12-26 - A tool that lets you generate wordlists by user profiling data such as birthday, nickname, address, name of a pet or relative etc.
* [StringZilla](https://github.com/ashvardanian/StringZilla) ⭐ 3,421 | 🐛 49 | 🌐 C | 📅 2026-03-23 - Fastest string sort, search, split, and shuffle for long strings and multi-gigabyte files in Python and C.
* [Mentalist](https://github.com/sc0tfree/mentalist) ⭐ 1,971 | 🐛 9 | 🌐 Python | 📅 2026-03-30 - Mentalist is a graphical tool for custom wordlist generation. It utilizes common human paradigms for constructing passwords and can output the full wordlist as well as rules compatible with Hashcat and John the Ripper.
* [anew](https://github.com/tomnomnom/anew) ⭐ 1,622 | 🐛 9 | 🌐 Go | 📅 2024-01-12 - Append lines from stdin to a file, but only if they don't already appear in the file. Outputs new lines to stdout too, making it a bit like a tee -a that removes duplicates.
* [bopscrk](https://github.com/r3nt0n/bopscrk) ⭐ 1,073 | 🐛 7 | 🌐 Python | 📅 2024-09-07 - Generate smart and powerful wordlists for targeted attacks. Includes song lyrics fetching and different transforms.
* [duplicut](https://github.com/nil0x42/duplicut) ⭐ 967 | 🐛 7 | 🌐 C++ | 📅 2025-11-04 - Remove duplicates from MASSIVE wordlist, without sorting it (for dictionary-based password cracking).
* [Elpscrk](https://github.com/D4Vinci/elpscrk) ⭐ 930 | 🐛 2 | 🌐 Python | 📅 2024-10-14 - Elpscrk is like cupp, but it's based on permutations and statistics while being memory efficient.
* [kwprocessor](https://github.com/hashcat/kwprocessor) ⭐ 600 | 🐛 7 | 🌐 C | 📅 2025-08-19 - Advanced keyboard-walk generator with configureable basechars, keymap and routes.
* [maskprocessor](https://github.com/hashcat/maskprocessor/) ⭐ 499 | 🐛 14 | 🌐 C | 📅 2022-06-20 - High-performance word generator with a per-position configureable charset.
* [princeprocessor](https://github.com/hashcat/princeprocessor) ⭐ 486 | 🐛 9 | 🌐 C | 📅 2023-10-30 - Standalone password candidate generator using the PRINCE algorithm.
* [Gorilla](https://github.com/d4rckh/gorilla) ⭐ 390 | 🐛 5 | 🌐 Rust | 📅 2026-02-01 - Tool for generating wordlists or extending an existing one using mutations.
* [statsprocessor](https://github.com/hashcat/statsprocessor/) ⭐ 188 | 🐛 1 | 🌐 C | 📅 2023-10-27 - Word generator based on per-position markov-chains.
* [TTPassGen](https://github.com/tp7309/TTPassGen) ⭐ 169 | 🐛 1 | 🌐 Python | 📅 2025-06-11 - Flexible and scriptable password dictionary generator which supportss brute-force, combination, complex rule modes etc.
* [Keyboard-Walk-Generators](https://github.com/Rich5/Keyboard-Walk-Generators) ⭐ 149 | 🐛 0 | 🌐 Python | 📅 2016-02-16 - Generate Keyboard Walk Dictionaries for cracking.
* [token-reverser](https://github.com/dariusztytko/token-reverser) ⭐ 110 | 🐛 1 | 🌐 Python | 📅 2020-05-20 - Words list generator to crack security tokens.
* [Rling](https://github.com/Cynosureprime/rling) ⭐ 95 | 🐛 0 | 🌐 C | 📅 2026-04-09 - RLI Next Gen (Rling), a faster multi-threaded, feature rich alternative to rli found in hashcat utilities.
* [common-substr](https://github.com/sensepost/common-substr) ⭐ 65 | 🐛 0 | 🌐 Go | 📅 2020-06-28 - Simple tool to extract the most common substrings from an input text. Built for password cracking.
* [Rephraser](https://github.com/travco/rephraser) ⭐ 63 | 🐛 2 | 🌐 Python | 📅 2022-03-15 - A Python-based reimagining of Phraser using Markov-chains for linguistically-correct password cracking.
* [Phraser](https://github.com/Sparell/Phraser) ⭐ 52 | 🐛 1 | 🌐 C++ | 📅 2015-12-25 - Phraser is a phrase generator using n-grams and Markov chains to generate phrases for passphrase cracking.
* [WikiRaider](https://github.com/NorthwaveSecurity/wikiraider) ⭐ 45 | 🐛 5 | 🌐 Python | 📅 2024-02-02 - WikiRaider enables you to generate wordlists based on country specific databases of Wikipedia.
* [Gramify](https://github.com/TheWorkingDeveloper/gramify) ⭐ 34 | 🐛 2 | 🌐 Python | 📅 2024-06-27 - Create n-grams of wordlists based on words, characters, or charsets to use in offline password attacks and data analysis.
* [maskuni](https://github.com/flbdx/maskuni) ⭐ 6 | 🐛 0 | 🌐 C++ | 📅 2022-08-07 - A standalone fast word generator in the spirit of hashcat's mask generator with unicode support.
* [accent\_permutator](https://github.com/cyclone-github/accent_permutator) ⚠️ Archived - A tool to transform characters from ASCII / UTF-8 to accented characters such as "o" to "ò".
* [Crunch](https://sourceforge.net/projects/crunch-wordlist/) - Crunch is a wordlist generator where you can specify a standard character set or a character set you specify. Crunch can generate all possible combinations and permutations.
* [PTT](https://github.com/JakeWnuk/ptt) - The Password Transformation Tool (ptt) is a versatile utility designed for password cracking. It facilitates the creation of custom rules and transformations, as well as the generation of wordlists. This tool supports processing data from files, URLs, and standard input, streamlining cracking workflows.

## Wordlists

### Laguage specific

* [French Wordlists](https://github.com/clem9669/wordlists) ⭐ 319 | 🐛 5 | 📅 2026-04-11 - This project aim to provide french word list about everything a person could use as a base password.
* [Danish Wordlists](https://github.com/narkopolo/danish-wordlists) ⭐ 30 | 🐛 0 | 📅 2023-01-11 - Collection of danish wordlists for cracking danish passwords.
* [Danish Phone Wordlist Generator](https://github.com/narkopolo/danish_phone_wordlist_generator) ⭐ 8 | 🐛 0 | 🌐 Python | 📅 2022-05-24 - This tool can generate wordlists of Danish phone numbers by area and/or usage (Mobile, landline etc.) Useful for password cracking or fuzzing Danish targets.
* [Albanian wordlist](https://github.com/its0x08/albanian-wordlist) ⭐ 7 | 🐛 0 | 📅 2023-01-05 - A mix of names, last names and some albanian literature.

### Other

* [Packet Storm Wordlists](https://packetstormsecurity.com/Crackers/wordlists/page1/) - A substantial collection of different wordlists in multiple languages.
* [Rocktastic](https://labs.nettitude.com/tools/rocktastic/) - Includes many permutations of passwords and patterns that have been observed in the wild.
* [RockYou2021](https://github.com/ohmybahgosh/RockYou2021.txt) ⭐ 996 | 🐛 4 | 📅 2024-03-10 -  RockYou2021.txt is a MASSIVE WORDLIST compiled of various other wordlists.
* [WeakPass](https://weakpass.com/) - Collection of large wordlists.

## Specific file formats

### PDF

* [pdfrip](https://github.com/mufeedvh/pdfrip) ⭐ 1,335 | 🐛 15 | 🌐 Rust | 📅 2026-03-26 - A multi-threaded PDF password cracking utility equipped with commonly encountered password format builders and dictionary attacks.

### JKS

* [JKS private key cracker](https://github.com/floyd-fuh/JKS-private-key-cracker-hashcat) ⭐ 189 | 🐛 0 | 🌐 Java | 📅 2020-09-21 - Cracking passwords of private key entries in a JKS file.

### ZIP

* [bkcrack](https://github.com/kimci86/bkcrack) ⭐ 2,097 | 🐛 14 | 🌐 C++ | 📅 2026-03-28 - Crack legacy zip encryption with Biham and Kocher's known plaintext attack.
* [frackzip](https://github.com/hyc/fcrackzip) ⚠️ Archived - Small tool for cracking encrypted ZIP archives.

## Machine Learning / AI

* [neural network cracking](https://github.com/cupslab/neural_network_cracking) ⭐ 242 | 🐛 16 | 🌐 JavaScript | 📅 2019-12-02 - Code for cracking passwords with neural networks.
* [rulesfinder](https://github.com/synacktiv/rulesfinder) ⭐ 115 | 🐛 3 | 🌐 Rust | 📅 2023-08-18 - This tool finds efficient password mangling rules (for John the Ripper or Hashcat) for a given dictionary and a list of passwords.
* [PassGPT](https://github.com/javirandor/passgpt) ⭐ 89 | 🐛 3 | 🌐 Python | 📅 2025-03-13 - PassGPT is a GPT-2 model trained from scratch on password leaks.
* [RNN-Passwords](https://github.com/gehaxelt/RNN-Passwords) ⭐ 87 | 🐛 0 | 📅 2021-03-28 - Using the char-rnn to learn and guess passwords.
* [adams](https://github.com/TheAdamProject/adams) ⭐ 21 | 🐛 2 | 🌐 C | 📅 2024-05-07 - Reducing Bias in Modeling Real-world Password Strength via Deep Learning and Dynamic Dictionaries.
* [SePass: Semantic Password Guessing using k-nn Similarity Search in Word Embeddings](https://github.com/Knuust/SePass) ⭐ 3 | 🐛 0 | 🌐 Python | 📅 2022-02-25 - A password guessing method that utilizes word embeddings to discover and exploit semantic correlations in password lists.

## Research

### Articles and Blog Posts

* [Optimizing Wordlists with Masks](https://jakewnuk.com/posts/optimizing-wordlists-w-masks/)
* [Purple Rain Attack - Password Cracking With Random Generation](https://www.netmux.com/blog/purple-rain-attack)
* [Smashing Hashes with Token Swapping Attacks](https://jakewnuk.com/posts/token-swapping-attack/)
* [Bcrypt at 25: A Retrospective on Password Security](https://www.usenix.org/publications/loginonline/bcrypt-25-retrospective-password-security)

### Papers

* [PassGPT: Password Modeling and (Guided) Generation with LLMs](https://arxiv.org/abs/2306.01545)
* [Password Cracking Using Probabilistic Context-Free Grammars (2009)](https://www.researchgate.net/publication/220713709_Password_Cracking_Using_Probabilistic_Context-Free_Grammars)
* [Fast, Lean, and Accurate: Modeling Password Guessability Using Neural Networks (2016)](https://www.usenix.org/conference/usenixsecurity16/technical-sessions/presentation/melicher)
* [PassGAN: A Deep Learning Approach for Password Guessing (2017)](https://arxiv.org/pdf/1709.00440)
* [GENPass: A General Deep Learning Model for Password Guessing with PCFG Rules and Adversarial Generation (2018)](https://ieeexplore.ieee.org/document/8422243)
* [Generating Optimized Guessing Candidates toward Better Password Cracking from Multi-Dictionaries Using Relativistic GAN (2020)](https://www.mdpi.com/2076-3417/10/20/7306/htm)
* [Reducing Bias in Modeling Real-world Password Strength via Deep Learning and Dynamic Dictionaries (2020)](https://arxiv.org/abs/2010.12269)
* [PassFlow: Guessing Passwords with Generative Flows (2021)](https://arxiv.org/abs/2105.06165)
* [GNPassGAN: Improved Generative Adversarial Networks For Trawling Offline Password Guessing (2022)](https://arxiv.org/pdf/2208.06943)
* [The Revenge of Password Crackers: Automated Training of Password Cracking Tools (2022)](https://doi.org/10.1007/978-3-031-17146-8_16)
* [A Systematic Review on Password Guessing Tasks (2023)](https://doi.org/10.3390/e25091303)
* [Harder, better, faster, stronger: Optimising the performance of context-based password cracking dictionaries (2023)](https://doi.org/10.1016/j.fsidi.2023.301507)
* [Confident Monte Carlo: Rigorous Analysis of Guessing Curves for Probabilistic Password Models (2023)](https://ieeexplore.ieee.org/stamp/stamp.jsp?tp=\&arnumber=10179365)
* [Improving Real-world Password Guessing Attacks via Bi-directional Transformers (2023)](https://www.usenix.org/conference/usenixsecurity23/presentation/xu-ming)
* [Mangling Rules Generation With Density-Based Clustering for Password Guessing (2023)](https://annas-archive.pk/scidb/10.1109/tdsc.2022.3217002/)
* [No Single Silver Bullet: Measuring the Accuracy of Password Strength Meters (2023)](https://www.usenix.org/system/files/usenixsecurity23-wang-ding-silver-bullet.pdf)
* [Optimizing The Computation Of Password Hashes (2023)](https://helda.helsinki.fi/server/api/core/bitstreams/23a37f74-a162-4473-b894-5da77f0627d1/content)
* [PGTCN: A Novel Password-Guessing Model Based On Temporal Convolution Network (2023)](https://annas-archive.pk/scidb/10.1016/j.jnca.2023.103592/)
* [Towards a Rigorous Statistical Analysis of Empirical Password Datasets (2023)](https://ieeexplore.ieee.org/document/10179431)
* [Enhancing The Resistance Of Password Hashing Using Binary Randomization Through Logical Gates (2024)](http://doi.org/10.11591/ijece.v14i5.pp5400-5407)
* [GuessFuse: Hybrid Password Guessing With Multi-View (2024)](https://ieeexplore.ieee.org/document/10466588)
* [PassRVAE: Improved Trawling Attacks via Recurrent Variational Autoencoder (2024)](https://dl.acm.org/doi/10.1145/3673277.3673295)
* [Prob-Hashcat: Accelerating Probabilistic PasswordGuessing with Hashcat by Hundreds of Times (2024)](https://dl.acm.org/doi/epdf/10.1145/3678890.3678919)
* [Reinforcing Cybersecurity With Bloom Filters: A Novel Approach To Password Cracking Efficiency (2024)](https://doi.org/10.1186/s13635-024-00183-2)
* [Beyond The Dictionary Attack: Enhancing Password Cracking Efficiency Through Machine Learning-Induced Mangling Rules (2025)](https://doi.org/10.1016/j.fsidi.2025.301865)
* [MAYA: Addressing Inconsistencies in Generative Password Guessing through a Unified Benchmark (2025)](https://arxiv.org/abs/2504.16651)
* [Password Guessing Using Large Language Models (2025)](https://www.usenix.org/system/files/usenixsecurity25-zou-yunkai.pdf)
* [PassRecover: A Multi-FPGA System for End-to-End Offline Password Recovery Acceleration (2025)](https://doi.org/10.3390/electronics14071415)
* [When Intelligence Fails: An Empirical Study on Why LLMs Struggle with Password Cracking (2025)](https://arxiv.org/abs/2510.17884)
* [Success Rates Doubled with Only One Character: Mask Password Guessing (2025)](https://doi.org/10.14722/ndss.2026.241059)
* [PGMaP: Password Generation Based On Mask Prediction (2026)](https://linkinghub.elsevier.com/retrieve/pii/S0957417426002319)
* [Improving targeted password guessing attacks by using personally identifiable information and old password (2026)](https://doi.org/10.1186/s42400-025-00430-0)

### Talks

* [BSides Cayman Islands 2024 - No Cap Cracking: Improving Offline Hash Recovery Methodologies](https://jakewnuk.com/static/No%20Cap%20Cracking%20Improving%20Offline%20Hash%20Recovery%20Methodologies.pdf)
* [BSides Cayman Islands 2023 - Leveling Up Password Attacks with Breach Data](https://jakewnuk.com/static/Leveling%20Up%20Password%20Attacks%20with%20Breach%20Data.pdf)
* [DEF CON Safe Mode Password Village - Getting Started with Hashcat](https://www.youtube.com/watch?v=MBTJ8f6Fsmg)
* [DEF CON Safe Mode Password Village - Jeremi Gosney - Cracking at Extreme Scale](https://www.youtube.com/watch?v=4Ell1Tt23NI)
* [DEF CON 28 Safe Mode Password Village – 'Let's Crack RockYou Without Using rockyou txt'](https://www.youtube.com/watch?v=8FtXntEsZdU)
* [SecTor 2019 - Will Hunt - Hashes, Hashes Everywhere, But All I See Is Plaintext](https://sector.ca/sessions/hashes-hashes-everywhere-but-all-i-see-is-plaintext/)
* [Tailored, Machine Learning-driven Password Guessing Attacks and Mitigation at DefCamp](https://www.youtube.com/watch?v=iK6ZbD6v9Gg)
* [UNHash - Methods for better password cracking](https://media.ccc.de/v/31c3_-_5966_-_en_-_saal_1_-_201412292245_-_unhash_-_methods_for_better_password_cracking_-_tonimir_kisasondi)
* [USENIX Security '23 - No Single Silver Bullet: Measuring the Accuracy of Password Strength Meters](https://www.youtube.com/watch?v=0vhoAaqGYV8)
* [USENIX Security '23 - Improving Real-World Password Guessing Attacks via Bi-Directional Transformers](https://www.youtube.com/watch?v=kE7dEUcPtU0)
* [USENIX Security '21 - Reducing Bias in Modeling Real-world Password Strength via Deep Learning and Dynamic Dictionaries](https://www.youtube.com/watch?v=Jvp3UTdCeag)
* [USENIX Security '16 - Fast, Lean, and Accurate: Modeling Password Guessability Using Neural Networks](https://www.youtube.com/watch?v=GgaZ_LxsL_8)
