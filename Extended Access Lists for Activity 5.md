


Standard ACL
---

| Device  | Permit/Deny | Source IP         | Source Interface | Source Ports | Destination Network | Destination Port | Direction |
| ------- | ----------- | ----------------- | ---------------- | ------------ | ------------------- | ---------------- | --------- |
| DMZ     | Permit      | 192.39.101.128/28 | S0/1/0           | *            | *                   | *                | Out       |
| Servers | Permit      | 10.4.15.0/24      | S0/1/0           | *            | *                   | *                | Out       |
| Desktop | Permit      | 10.4.5.0/24       | S0/1/0           | *            | *                   | *                | Out       |



Extended Access List
---
| Device   | Permit/Deny | Source IP | Source Interface | Source Ports | Destination Network | Destination Port | Direction |
| -------- | ----------- | --------- | ---------------- | ------------ | ------------------- | ---------------- | --------- |
| DNS      | Permit      | *         | S0/1/0           | *            | 192.39.101.130      | 53/udp           | In        |
| DNS      | Permit      | *         | S0/1/0           | *            | 192.39.101.130      | 53/TCP           | In        |
| Web1     | Permit      | *         | S0/1/0           | *            | 192.39.101.131      | 80/HTTP          | In        |
| Web1     | Permit      | *         | S0/1/0           | *            | 192.39.101.131      | 443/HTTPS        | In        |
| Web2     | Permit      | *         | S0/1/0           | *            | 192.39.101.133      | 80/HTTP          | In        |
| Web2     | Permit      | *         | S0/1/0           | *            | 192.39.101.133      | 443/HTTPS        | In        |
| FTP      | Permit      | *         | S0/1/0           | *            | 192.39.101.132      | 21/FTP           | In        |
| Internet | Deny        | *         | S0/1/0           | *            | 10.0.0.0/8          | *                | In        |
