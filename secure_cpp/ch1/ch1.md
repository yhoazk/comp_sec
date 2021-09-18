
# CH1
Computer systems are not vulnerable to attack, we are vulnerable to attack through our computer systems.

Blaster worm exploits RPC running on TCP port 135, specifically windows implementation which was patched before the release.
Even when the fix was already available and the worm was developed after the release of the patch infected 1M PCs at a rate of 100k per hour.

Blaster checks if the computer was already infected, if it was the worm does not infect the computer a second time. Otherwise modifies the registry key: `HKEY_LOCAL_MACHINE\SOFTWARE\Microsoft\Windows\CurrentVersion\Run` so that the worm gets executed when windows is started. Once it is installed generates a random IP and attempts to infect that computer. This worm was present onf windows xp and windows 200. Blaster worm listens to UDP:69  fora request of an infected computer, then sends the mblast file which executes the worm.

This worm uses `cmd.exe` to create a backdoor remote shell process that listens on TCP 4444. Allowing remote command execution.

Since the DCOM RPC buffer overflow vulnerability was present in the process `svchost` it caused the system to become unstable and hang.
On windows XP and 2003 the default actions was to initiate a reboot.

The error that caused this was un checked while-loop which was not bounded. Rather the stop condition was checking for the end of the string.

```cpp
char* temp = path;
while (*temp != '\0') {
    *result++ = *temp++;
}
```

---
DCOM : Distributed component object model
RPC: remote procedure call is an interprocess communication mechanism that allows a program running on one computer to execute code on a remote system. 
SYN flood: Method used as a DoS sending SYN packets to every port on the setver using fake IP addresses.


## CH1.1

the threat in security systems is defined as a person, group or organizazion, or foreign power that has been the source of past attacks or may be the source of future attacks.

- Hackers: MOtivated by curiosity and peer recognition
- Insiders: current or former employee motivated by financial gain or revenge.
- Criminals: Members of organized crime who hope to profit. M
- Comptetitive intelligence professionals: Corporate spies
- Terrorist: Their goal is to coerce a goverment or its people for a political or social objective
- Information warriors: nations with cyber warfare capabilities.

## CH1.2

computer security prevents attackers from achieving objectives through unauthorized access or unauthorized use of computers or networks.
Definition from RFC 2828: A set of rules and practices that specify or regulate how a system or organization provides security services to protect sensitive and critical system resources.
Definitions: 
- Vulnerability: A set of conditions that allows an attacker to violate an explicit or implicit security policy
- Security flaw: a software defect that poses a potential security risk
- exploit: An exploit is a piece of software or technique that takes advantage of a security vulnerability to violate an explicit or implicit security policy
- Mitigations: Are methods, techniques, processes, tools or runtime libraries that can prevent or limit exploits against vulnerabilties.


## CH1.3

C was derived from the typeless language B, which in turn was derived from BCPL. C can be seen as B with types. Descendants from C include Concurrent C, Objective C C* and speciylly C++. From his descendants C++ has been the most widely adopted. Bjarne Stroustrup added features  to C and formed what he called C with classes.

The problem with C could be attributed to the portability expected from the language. This portability requires the logic to be encoded at a level of abstraction independent of the undelying arch and transformed or compiled into the underlying representation. Problems arise from an imprecise undestanding of the semantics of these logical abstractions and how they translate into machine-level instructions. This lack of undestanding leads to mismatched assumptions, security flaws and vulnerabilities.

This characteristic leads to vulnerabilities when programmes fail to implement required logic because they assume it is handled by C, when it is not. This problem is magnified when the programer is familir with superficially similar langugagess leading them to believe that C also protects them as other languages do. 

Another characteristic of C is the lack of type safety. Type safety consists of two attributes: _preservation and progress_.
Preservation dictates that if a variable `x` has type `t` and `x` evaluates to a value `v` then `v` also has type `t`. Progress tells us that evaluation of an expression foes not get stuck in any unexpected way: either we have a value, or there is a way to proceed. 
In general type safety implies that any operation on a particular type resuls in another calue of that type.


## Ch1.4

operating systems used: Windows (XP, server 2003, 200, Me, 98, 95, NT workstation, NT server). Linux.

Compilers Visual C++ and GCC


## summary

everything on the list of the SANS TOP 20 internet security vulnerabiity list is the result of poor coding, testing and sloppy software engineering. These are not bleeding edge problems as an innocent bystander might assume. Technical solutions for all of them exist, but the are symply not implemented.


