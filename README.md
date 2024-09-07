# Go assembler

> [Also, perhaps most important: it is how we talk about the machine
Knowing assembly, even a little, means understanding computers better](https://youtu.be/KINIAgRpkDA?t=101)
> (Rob Pike)

## Задание

В данном домашнем задании вам предлагается реализовать несколько функций, используя ассемблер Go. При этом нужно будет поддержать решения для arm64 или amd64.

**SliceSum**

`func SumSlice(x []int64) int64`

Необходимо реализовать функцию, возвращающую сумму переданного слайса

**LowerBound**

`func LowerBound(slice []int64, value int64) int64`

Необходимо реализовать одну из вариаций бинарного поиска - [LowerBound](https://en.wikipedia.org/wiki/Upper_and_lower_bounds)

**Fibonacci**

`func Fibonacci(n uint64) uint64`

Необходимо реализовать функцию, которая возвращает n-е число Фибоначчи

**WordCount**

`func WordCount(data []rune) int64`

Необходимо реализовать функцию, которая считает количество слов в переданной строке (separator - unicode.IsSpace)

## Особенности реализации

- Различие регистров, инструкций и соглашений для разных архитектур (amd64/arm64)
- Обработка слайса в качестве аргумента функции
- Директивы и идиоматичные части сигнатуры функции на ассемблере

# Дополнительные материалы

- [The manual for Plan9 asm](https://9p.io/sys/doc/asm.html)
- [Guide to Go's Assembler](https://go.dev/doc/asm)
- [Optimising go code with asm](https://www.jamesbowman.me/post/optimising-go-code-with-assembler/)
- [Rob Pike - The Design of the Go Assembler](https://www.youtube.com/watch?v=KINIAgRpkDA)
- [A Foray Into Go Assembly Programming](https://blog.sgmansfield.com/2017/04/a-foray-into-go-assembly-programming/)
- [Slice arguments in go asm](https://mmcloughlin.com/posts/golang-asm-slice-arg)