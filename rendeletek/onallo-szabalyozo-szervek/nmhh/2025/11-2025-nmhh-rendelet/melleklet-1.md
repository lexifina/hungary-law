1. melléklet a 11/2025. (XII. 10.) NMHH rendelethez

A CBE, CBC adatátvitel műszaki alapkövetelményei

1. Az OSI-modell 7. rétegén (alkalmazási réteg) a HTTPS protokollt kell alkalmazni az RFC 2818 szerint.

2. A HTTPS titkosítását és hitelesítését a TLS1.2 (hosszú távon 1.3) protokoll biztosítja az RFC 8446 szabványnak megfelelően.

3. A TCP-csomagokat az OSI 3. rétegén az IPv4 protokoll kezeli.

4. A site-to-site VPN javasolt konfigurációs paraméterei az alábbiak:

|  | A | B |

| 1 | Peer IP Primary | a fizikai kapcsolat módjától függ |

| 2 | Port | UDP/500; UDP/4500; IP 50 ESP |

| 3 | VPN Product | a fizikai kapcsolat módjától függ |

| 4 | IKE Policy | IKev2 Preferred |

| 5 | Message Encryption algorithm | AES256 |

| 6 | Message integrity algorithm | SHA256 |

| 7 | Peer Authentication Method | PSK |

| 8 | DH-Group | 14 |

| 9 | IKE Lifetime | 21600 |

| 10 | Mechanism for payload encryption | E S P |

| 11 | ESP Transform | AES 256 |

| 12 | Data Integrity | S H A 256 |

| 13 | Security Association (SA) Lifetime | 3600 (or less) |

| 14 | Perfect Forwarding Secrecy (PFS) | Group 14 |
