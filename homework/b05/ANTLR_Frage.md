**ANTLR – Frage:**



Vergleichen Sie das so erzeugte Syntax-Highlighting mit den Varianten aus Blatt 04. Wo liegen die Unterschiede, und wodurch entstehen diese? Welche der Varianten ist aufwändiger in der Implementierung?



Ich habe zuvor ausschließlich den Regex-Highlighter implementiert. Der meiner Meinung nach größte Unterschied besteht darin, dass beim ANTLR-Ansatz die MiniJavaToken nicht selbst definiert werden müssen, da bereits Zugriff auf die MiniJava.g4-Grammatikdatei besteht.



Ich empfand den Regex-Highlighter insgesamt als einfacher zu implementieren. Allerdings sollte der ANTLR-basierte Token-Collector theoretisch weniger Implementierungsaufwand verursachen, da die Tokenisierung bereits durch ANTLR vorgegeben ist.

