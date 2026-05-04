# isc-cissp-official-practice-tests-4th-edition
## ISC2 CISSP Certified Information Systems Security Professional Official Practice Tests (4th Edition)
1. Login to `VitalSource` as `martinmcc5804@gmail.com`
2. Scrape from web: `https://bookshelf.vitalsource.com/reader/books/9781394255085?library_return_url=https%3A%2F%2Fbookshelf.vitalsource.com%2Fhome%2Fdashboard`
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