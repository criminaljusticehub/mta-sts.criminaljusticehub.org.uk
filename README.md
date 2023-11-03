<h1 align="center">
  <br>
  📩 MTA Strict Transport Security (MTA-STS) policy for the Criminal Justice Hub (CJH).
  <br>
</h1>

<h4 align="center">

MTA-STS is a security standard for secure e-mail delivery. E-mail servers that send inbound e-mail to the Criminal Justice Hub will be able to detect that our e-mail server supports SMTP-over-TLS via `STARTTLS` (also known as [Opportunistic TLS](https://en.wikipedia.org/wiki/Opportunistic_TLS)) before opening the actual connection.

In case the sending e-mail server is not able to initiate a secure connection, it will end the connection to enforce transport layer encryption. This mitigates [Man-in-the-middle](https://en.wikipedia.org/wiki/Man-in-the-middle_attack) DNS and SMTP [downgrade attacks](https://en.wikipedia.org/wiki/Downgrade_attack) that would allow an attacker to read or manipulate e-mail in transit.
