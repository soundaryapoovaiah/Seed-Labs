📘 Overview

This lab focused on exploiting and understanding Cross-Site Scripting (XSS) vulnerabilities using a vulnerable version of the Elgg social networking platform. By crafting malicious JavaScript code, we explored how attackers can inject scripts into web applications, steal session cookies, forge requests, and propagate self-replicating worms. The lab also covered Content Security Policy (CSP) as a modern countermeasure to defend against such attacks.

🧪 Key Lab Tasks

Task 1: Injected basic JavaScript payloads to display alert messages in a user's browser.

Task 2: Displayed session cookies through malicious JavaScript embedded in a profile.

Task 3: Stole session cookies by sending them to an attacker’s machine using a fake <img> tag.

Task 4: Forged HTTP requests from a victim's browser to make them unknowingly add the attacker as a friend.

Task 5: Modified a victim’s profile using forged POST requests, injecting new values into form fields.

Task 6: Created a self-propagating XSS worm that replicates itself across profiles and adds the attacker as a friend, emulating the famous Samy worm on MySpace.

Task 7: Evaluated the effectiveness of Content Security Policy (CSP) using Apache and PHP-based server configurations to restrict script execution.

💡 What I Learned

How XSS attacks work—including reflected, stored, and DOM-based variants.

Crafting and injecting malicious JavaScript payloads to manipulate browser behavior.

Using HTTP inspection tools (like HTTP Header Live and Firefox Developer Tools) to study request headers, cookies, and form submission behavior.

Exploiting same-origin policy flaws to steal session data and forge user actions.

Building and deploying self-replicating worms in a web application.

Implementing CSP rules to prevent inline scripts and untrusted source execution, mitigating real-world XSS threats.

🌍 Real-World Applications

Cybersecurity Roles (Pentesting/Red Teaming): These skills are crucial for simulating XSS attacks and identifying client-side vulnerabilities in web apps.

Frontend/Backend Web Development: Understanding XSS attack vectors helps developers write secure code using safe templating practices and encoding strategies.

Security Engineering: Applying Content Security Policy as a defense-in-depth strategy to prevent browser-based exploits and reduce attack surfaces.

Bug Bounty Hunting: XSS is one of the most commonly reported vulnerabilities in web bug bounty programs like HackerOne and Bugcrowd.
