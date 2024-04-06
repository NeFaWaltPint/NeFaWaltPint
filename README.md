```Golang
package main

import (
	"fmt"

	"github.com/NeFaWaltPint/xd"
)

func main() {
	person := xd.PersonData{
		Name:       "Neider Fabian Walteros Pinto",
		Origin:     "Yopal, Colombia",
		Profession: "Electronic Engineer",
		ProgrammingLanguages: []string{
			"C", "TypeScript", "Go", "Bash", "Python", "PHP", "Ladder", "CNC",
		},
		Software: []string{
			"Labview", "Matlab", "SolidWorks", "Proteus Design", "NI Multisim", "OnShape",
			"CorelDraw", "Photoshop",
		},
		Projects: []string{
			"Home automation using IoT devices and web implementations from scratch", 
			"Acquisition and digital processing of myoelectric signals",
		},
		Interests: []string{
			"Cycling", "Photography", "GNU/Linux enthusiast",
			"Listening and explore music (rock, metal, postrock, shoegaze, postpunk, synth pop...)",
			"Watching movies and series (cult classics, thriller, sci-fi...)",
			"Space exploration, physics and scientific dissemination...",
		},
	}

	fmt.Printf("Hello, my name is %s, I'm from %s. I'm a %s.\n", person.Name, person.Origin,
		person.Profession)

	fmt.Println("I have skills in the following programming languages:")
	xd.PrintList(person.ProgrammingLanguages)

	fmt.Println("I'm also proficient in using the following software:")
	xd.PrintList(person.Software)

	fmt.Println("Projects or ideas I've worked on:")
	xd.PrintList(person.Projects)

	fmt.Println("In my free time, I enjoy:")
	xd.PrintList(person.Interests)
}
```
