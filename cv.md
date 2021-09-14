# Arthur Zhassymov

## Contacts
phone:  +7 (701) 3877333

## About

Hi there! I'm a software developer.
  
I'm interested in developing web applications and services. My commercial development experience started in May 2021.  

I __*love*__ programming and strive to write high performance, reliable and clean code.
  
I believe that thanks to modern technology, we can make this world a better place.

## Knowledges and skills

[<img alt="MongoDB" src="https://cdn.svgporn.com/logos/go.svg" style="height: 40px; margin: 10px;"/>](https://golang.org/)
[<img alt="MongoDB" src="https://cdn.svgporn.com/logos/mongodb.svg" style="height: 40px; margin: 10px;"/>](https://www.mongodb.com/)
[<img alt="PostgreSQL" src="https://cdn.svgporn.com/logos/postgresql.svg" style="height: 40px; margin: 10px;"/>](https://www.postgresql.org/)
[<img alt="RabbitMQ" src="https://cdn.svgporn.com/logos/rabbitmq-icon.svg" style="height: 40px; margin: 10px;"/>](https://www.rabbitmq.com/)
[<img alt="gRPC" src="https://cncf-branding.netlify.app/img/projects/grpc/icon/color/grpc-icon-color.svg" style="height: 40px; margin: 10px;"/>](https://grpc.io/)
[<img alt="REST" src="https://cdn.svgporn.com/logos/json.svg" style="height: 40px; margin: 10px;"/>](https://en.wikipedia.org/wiki/Representational_state_transfer)
[<img alt="git" src="https://cdn.svgporn.com/logos/git-icon.svg" style="height: 40px; margin: 10px;"/>](https://git-scm.com/)
[<img alt="GoLand" src="https://resources.jetbrains.com/storage/products/goland/img/meta/goland_logo_300x300.png" style="height: 40px; margin: 10px;"/>](https://www.jetbrains.com/go/)
[<img alt="VS Code" src="https://cdn.svgporn.com/logos/visual-studio-code.svg" style="height: 40px; margin: 10px;"/>](https://code.visualstudio.com/)
[<img alt="Fedora" src="https://cdn.svgporn.com/logos/fedora.svg" style="height: 40px; margin: 10px;"/>](https://getfedora.org/)

## Learning

[<img alt="Javascript (JS)" src="https://cdn.svgporn.com/logos/javascript.svg" style="height: 40px; margin: 10px;"/>](https://en.wikipedia.org/wiki/JavaScript)
[<img alt="React" src="https://cdn.svgporn.com/logos/react.svg" style="height: 40px; margin: 10px;"/>](https://reactjs.org/)
[<img alt="Svelte" src="https://cdn.svgporn.com/logos/svelte-icon.svg" style="height: 40px; margin: 10px;"/>](https://svelte.dev/)

## Code examples

### Golang

```go
package main

import (
	"fmt"
	"sort"
	"strconv"
	"strings"
)

func Counter(s string) string {
	if len(s) == 0 {
		return ""
	}

	entries := make(map[rune]int)

	for _, char := range []rune(s) {
		entries[char]++
	}

	chars := make([]string, 0, len(entries))

	for char := range entries {
		chars = append(chars, string(char))
	}

	sort.Strings(chars)

	result := make([]string, 0, len(chars)*2)
	for _, str := range chars {
		char := []rune(str)[0]
		result = append(result, str, strconv.Itoa(entries[char]))
	}

	return strings.Join(result, "")
}

func main() {
	tests := []string{
		"aaabbbccccc",
		"aaabbbcccccaaaaa",
		"zzzzcccUUUuu",
		"ЯЯЯБББддд",
		"a",
	}

	for _, test := range tests {
		fmt.Println(test, Counter(test))
	}
}

```

### Javascript

```js
function reverseArray(array) {
    let result = [];
    for (let elem of array) result.unshift(elem)
    return result;
}

function reverseArrayInPlace(array) {
    for (let i = 0; i < Math.floor(array.length / 2); i++) {
        let temp = array[i]
        array[i] = array[array.length - 1 - i]
        array[array.length - 1 - i] = temp;
    }
}


console.log(reverseArray(["A", "B", "C"]));
// ["C", "B", "A"];

let arrayValue = [1, 2, 3, 4, 5];

reverseArrayInPlace(arrayValue);
console.log(arrayValue);
// [5, 4, 3, 2, 1]
```

## Work experience

- Technodom Operator, JSC
  - Golang Developer 
  - May 2021 - now
  - Stack:
    - Golang
    - microservices
    - gRPC
    - MongoDB
	- RabbitMQ

- Lawyer
  - September 2009 - May 2021

## Education

- [West Kazakhstan State University](https://wku.edu.kz/en/)
  - Bachelor of Laws
  - 2005 - 2009

- [alem](https://alem.school/)
  - Fullstack Developer
  - February 2020 - now

## Courses & certificates

- [Learning How to Learn, 2021](https://coursera.org/share/60dc31471dcca71e642afd35e2368d77)
- [Web services development with Golang, 2021](https://coursera.org/share/a4e76bd92e3f3a723d41e280283bad19)
- [Web Application Security, 2021](https://xakep.ru/)
- [Golang programming, 2020](https://stepik.org/cert/809216)
- [Introduction to Linux, 2020](https://stepik.org/cert/300369)
- [Python programming](https://stepik.org/cert/216559)
- [Professional HTML & CSS, level 1, 2018](https://assets.htmlacademy.ru/certificates/intensive/73/768969.pdf?1605190869&_ga=2.48561574.1272170262.1631629215-1460873961.1613326496)

## Languages

- Russian, native
- English, B1
