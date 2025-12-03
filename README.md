package main

import (
	"fmt"
	"log"
	"strconv"
)

/*func main() {
	x := 1
	yStr := "2"
	yInt, err := strconv.Atoi(yStr) //если получается преобразовать строку в число
	// мы получаем переменную , иначе - ошибку

	if err != nil { // если вернулась ошибка
		log.Fatal(err) // то завершаем программу
	}

	fmt.Println(x + yInt) // 3
}*/

func main() {

	x, yStr := 12., "2."
	yInt, err := strconv.ParseFloat(yStr, 64)
	if err != nil {
		log.Fatal(err)
	}
	fmt.Println(x - yInt) //10
}
