## Hello there 👋

```go
package main

import "fmt"

type SystemsEngineer struct {
	Name          string
	Code          []string
	AskMeAbout    []string
	Technologies  map[string]interface{}
	CloudServices map[string]interface{}
	CurrentFocus  string
	FunFact       string
}

func NewSystemsEngineer() SystemsEngineer {
	return SystemsEngineer{
		Name:       "Jeremy",
		Code:       []string{"Go", "Python", "Bash"},
		AskMeAbout: []string{"Cloud Computing", "DevOps", "System Design", "Tech Trends"},
		Technologies: map[string]interface{}{
			"FrontEnd":  []string{"HTML", "CSS", "JavaScript"},
			"BackEnd":   []string{"Go", "Python"},
			"DevOps":    []string{"Docker", "Kubernetes", "CI/CD"},
			"Databases": []string{"PostgreSQL", "MySQL"},
		},
		CloudServices: map[string]interface{}{
			"AWS":   []string{"EC2", "S3", "Lambda", "CloudWatch"},
			"Azure": []string{"VMs", "Blob Storage", "Functions"},
		},
		CurrentFocus: "Curently working on upskilling with CI/CD and GitOps tools like Jenkins, FluxCD, and ArgoCD.",
		FunFact:      "I'm 15% more productive when I have a cup of coffee while working!",
	}
}

func main() {
	me := NewSystemsEngineer()

	// Pretty-printing the struct content
	fmt.Printf("Hi! I'm %s. Here's a bit about me:\n", me.Name)
	fmt.Printf("  Languages I code in: %v\n", me.Code)
	fmt.Printf("  Ask me about: %v\n", me.AskMeAbout)
	fmt.Println("  Technologies I'm familiar with:")
	for category, items := range me.Technologies {
		fmt.Printf("  - %s: %v\n", category, items)
	}
	fmt.Println("  Cloud Services I work with:")
	for category, items := range me.CloudServices {
		fmt.Printf("  - %s: %v\n", category, items)
	}
	fmt.Printf("  Current Focus: %s\n", me.CurrentFocus)
	fmt.Printf("  Fun Fact: %s ☕\n", me.FunFact)
}
```

