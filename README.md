# isc-cissp-official-practice-tests-4th-edition
## ISC2 CISSP Certified Information Systems Security Professional Official Practice Tests (4th Edition)
1. Login to `VitalSource` as `martinmcc5804@gmail.com`
2. Scrape from web: https://bookshelf.vitalsource.com/reader/books/9781394255085?library_return_url=https%3A%2F%2Fbookshelf.vitalsource.com%2Fhome%2Fdashboard
- `Questions`
```
const text = Object.keys([...new Array(100)])
	.map(e=>parseInt(e)+1)
	.map(i=>{
		let q;
		if(i<10) q = `00${i}`;
		else if(i<100) q = `0${i}`;
		else q = `${i}`;
		const s = `#c01-ex-0${q}`;
		const e = document.querySelector(s);
		return `====\nQuestion ${q}:\n${e.innerHTML}`;
	})
	.join('\n');
console.log(text);
```
- `Answers`
```
const text = Object.keys([...new Array(100)])
	.map(e=>parseInt(e)+1)
	.map(i=>{
		let q;
		if(i<10) q = `00${i}`;
		else if(i<100) q = `0${i}`;
		else q = `${i}`;
		const s = `#bapp01-ex-0${q}`;
		return `====\Answer ${q}:\n${document.querySelector(s).innerText}`;
	})
	.join('\n\n');
console.log(text);
```
3. Create `MCQ Platform` as `MCQ Platform.html`
```
Create a `MCQ Platform.html` to provide a `MCQ Platform` for `Domain 1`.
- Question Types: `Many choose one` (radio), `Many choose one or many` (checkbox), `Mapping` (e.g. A-4;B-2;C-1;D-3)
- Score after submission
- Show summary report for the results, and also allow to export as CSV
```
## Fulfillment of CISSP working experiences
1. About `what I built`
- 🔴 `Year 1` to `Year3`
  - Develop a **web application** served as a _booking appointment system_ by **C# .NET**
  - Develop a **window form** served as a _query system_ in **C#**
  - Develop a **window form** served as a _socket server_ in **Java**
  - Code for a **web application** served as a _workflow system_ in **Java** (in **Springboot**) collaboratively
- 🔴 `Year 4` to `Year 6`
  - Develop a **web application** served as a _earthquake information dissemination application_ in **HTML**/**JS**/**CSS** (in **LAMP**), including input validation for earthquake data entry
  - Develop a **web application** served as a _locally felt information application_ via **JS** (in **MERN**), including assuring secure API in internal network protected by organization firewall
  - Fulfill **adhoc tasks** for _normal operations of the other systems_
2. About `how I secured it`
- 🔴 `Year 1` to `Year 3`
  - **Secure Software Lifecycle Management:** Managed the security of a **.NET** booking system and **Java-based** workflow application by implementing **_parameterized queries_** to protect against SQL injection and common web vulnerabilities (`Domain 8`).
- 🔴 `Year 4` to `Year 6`
  - **Application Security Testing & Validation:** Led the development earthquake information system for internal use, implementing rigorous **_client-side input validation_** and **_input encoding_** to mitigate Cross-Site Scripting (XSS) and injection risks (`Domain 8`).
  - **Network and API Security:** Architected and **_secured internal APIs_** within a **MERN** stack environment, ensuring secure communication through firewall policy alignment, network segmentation, and endpoint protection within the organizational perimeter (`Domain 4`).
  - **Security Operations & Maintenance:** Performed **_continuous security monitoring_** and ad-hoc **_vulnerability remediation_** for legacy systems to ensure ongoing availability and resilience of critical information dissemination services (`Domain 7`).
