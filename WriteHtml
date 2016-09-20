package main

import "os"

func main() {
	var row int
	var colsize int
	var column [8]string
	column[0] = "sNo "
	column[1] = "Name "
	column[2] = "1 "
	column[3] = "Rajesh "
	column[4] = "2 "
	column[5] = "Sindhu "
	column[6] = "3 "
	column[7] = "Aadhya "
	row = 4
	colsize = 2
	temp:=0
	var contents string
    
	file, err := os.Create("text.htm")
    if err != nil {
        return
    }
    defer file.Close()
	

	contents="<table border = 1>"
	for j := 0; j < row; j++ {
		contents+="<tr>"
		for i :=0; i < colsize; i++ {
			contents+="<td>" + column[temp] + "</td>"
			temp++
		}
		contents+="</tr>"
	}

	contents+="</table>"
    file.WriteString(contents)
}
