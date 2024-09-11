# Assembler-1
Целью данного проекта является разработка программы, которая будет моделировать работу ЭВМ для вычисления выражений в постфиксной форме. Программа имитирует вычислительную машину, в которой есть 1 регистр и 6 инструкций:
1.	LD A помещает операнд А в регистр;
2.	ST A помещает содержимое регистра в переменную А;
3.	AD A прибавляет содержимое переменной А к регистру;
4.	SB A вычитает содержимое переменной A из регистра;
5.	ML A умножает содержимое регистра на переменную A;
6.	DV A делит содержимое регистра на переменную A.
	На вход программы должно подаваться произвольное выражение в постфиксной форме записи, содержащее однобуквенные операнды латинского алфавита (А, В, С…) и операции +, -, * и /. Она должна напечатать последовательность инструкций, необходимых для вычисления выражения, и оставить результат в регистре. Также она должна использовать переменные в виде Tn в качестве временных.  Например, постфиксное выражение ABC*+DE-/ даст такую распечатку инструкций: 
LD B 		LD D
ML C 	  SB E
ST T1 	ST T3
LD A 	  LD T2
AD T1 	DV 23
ST T2 	ST T4
