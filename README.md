# SWE_2021_41_2024_2_week_6
---
## Week 4 Assignment
#### https://github.com/SeoyeonPark-skku/SWE_2021_41_2024_2_week_6.git
```python
def isHappy(n):
  while True:
    total = 0
    for digit in str(n):
      total += int(digit) ** 2
    n = total
    if n == 1:
      return True
    if n == 4:
      return False
```
### Description: 
#### This code checks if a number is "happy." It loops, repeatedly replacing the number with the sum of the squares of its digits. If the number becomes 1, it returns True, meaning the number is happy. If it reaches 4, it returns False, as 4 indicates an endless cycle, meaning the number is not happy.

---
```python
docker exec <container_name> cat /etc/os-release
```
### Explanation: 
#### This command executes cat /etc/os-release inside the Docker container named ossp-container. It displays details about the operating system running inside the container.\
### Ouput:
```python
PRETTY_NAME="Ubuntu 24.04.1 LTS"
NAME="Ubuntu"
VERSION_ID="24.04"
VERSION="24.04.1 LTS (Noble Numbat)"
VERSION_CODENAME=noble
ID=ubuntu
ID_LIKE=debian
HOME_URL="https://www.ubuntu.com/"
SUPPORT_URL="https://help.ubuntu.com/"
BUG_REPORT_URL="https://bugs.launchpad.net/ubuntu/"
PRIVACY_POLICY_URL="https://www.ubuntu.com/legal/terms-and-policies/privacy-policy"
UBUNTU_CODENAME=noble
LOGO=ubuntu-logo
```
```python
docker exec <container_name> git --version
```

```python
docker exec <container_name> python3 --version
```

```python
docker inspect --format="{{ .HostConfig.Binds }}" <container_name>
```
