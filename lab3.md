# Lab Report 3: Researching Commands 

## ```grep -r``` ([source](https://www.cyberciti.biz/faq/howto-use-grep-command-in-linux-unix/))
- Example 1
> $ grep -r 'Lucayans' .
> 
>./written_2/travel_guides/berlitz2/Bahamas-History.txt:Centuries before the arrival of Columbus, a peaceful Amerindian people who called themselves the Luccucairi had settled in the Bahamas. Originally from South America, they had traveled up through the Caribbean islands, surviving by cultivating modest crops and from what they caught from sea and shore. Nothing in the experience of these gentle people could have prepared them for the arrival of the Pinta, the Niña, and the Santa Maria at San Salvador on 12 October 1492. Columbus believed that he had reached the East Indies and mistakenly called these people Indians. We know them today as the Lucayans. Columbus claimed the island and others in the Bahamas for his royal Spanish patrons, but not finding the gold and other riches he was seeking, he stayed for only two weeks before sailing towards Cuba.
>
>./written_2/travel_guides/berlitz2/Bahamas-History.txt:The Spaniards never bothered to settle in the Bahamas, but the number of shipwrecks attest that their galleons frequently passed through the archipelago en route to and from the Caribbean, Florida, Bermuda, and their home ports. On Eleuthera the explorers dug a fresh-water well — at a spot now known as “Spanish Wells” — which was used to replenish the supplies of water on their ships before they began the long journey back to Europe with their cargoes of South American gold. As for the Lucayans, within 25 years all of them, perhaps some 30,000 people, were removed from the Bahamas to work — and die — in Spanish gold mines and on farms and pearl fisheries on Hispaniola (Haiti), Cuba, and elsewhere in the Caribbean.

The command ```grep -r``` with ```'pattern/words'``` and ```path```, what it's doing is grouping up the pattern or word with the current directory and all of it's subdirectories bascially a whole general search. It returns the file the word is found and the specific paragraph/lines of text if contains the word. 
- Example 2
> $ grep -r 'Amsterdam-Intro' . 
>
>  Binary file ./.git/index matches
> 
> ./berlitz2-wordcount.txt:   1498 written_2/travel_guides/berlitz2/Amsterdam-Intro.txt

The command ```grep -r``` with ```'pattern/words'``` and ```path``` same as the previous example, useful because it allows you to search for a pattern recursively in all files and directories within a given directory tree. 

## ```grep -c``` ([source](https://www.cyberciti.biz/faq/howto-use-grep-command-in-linux-unix/))
- Example 1
> $ grep -c 'island' ./written_2/travel_guides/berlitz2/Bermuda-WhereToGo.txt
> 
> 38

The command ```grep -c``` with ```'pattern/words'``` and ```path``` use the pattern to find the identical pattern/word in a gioven path file and counts how many times the pattern/word is found. Might use this option to find the total number of occurances of a pattern in a file. 

- Example 2  
> $ grep -c 'bad' ./written_2/travel_guides/berlitz2/Athens-WhereToGo.txt 
>  
> 1

The command ```grep -c``` with ```'pattern/words'``` and ```path```, same as the previous example but checking in another file. Useful because it allows you to count the number of occurrences of a pattern or keyword within a file or set of files. 

## ```grep -i``` ([source](https://www.cyberciti.biz/faq/howto-use-grep-command-in-linux-unix/))
- Example 1
> grep -i 'Bad' ./written_2/travel_guides/berlitz2/Athens-WhereToGo.txt
> 
> Eventually it was used as a powder magazine. In September 1687 Venetian forces threatened Athens and one of their mortars hit the Parthenon, igniting the powder inside. The resulting explosion badly damaged the structure and many other ancient buildings on the site. The center of the Parthenon was totally destroyed along with many columns and priceless carved friezes. Subsequent “licences” granted by the Ottomans to European nobles saw many prize friezes disappear to archaeological collections around Europe, including the Elgin marbles (ornately carved pediments) that were taken to London by Lord Elgin. Restoration of the temple has been almost constant since 1834.

The The command ```grep -i``` with ```'pattern/words'``` and ```path``` uses the given pattern and matches it to a given file. Prints out the matched file paragraph/lines. Useful for case-insensitive search. 
- Example 2 
> grep -i 'lucayans' ./written_2/travel_guides/berlitz2/Bahamas-History.txt
> 
> Centuries before the arrival of Columbus, a peaceful Amerindian people who called themselves the Luccucairi had settled in the Bahamas. Originally from South America, they had traveled up through the Caribbean islands, surviving by cultivating modest crops and from what they caught from sea and shore. Nothing in the experience of these gentle people could have prepared them for the arrival of the Pinta, the Niña, and the Santa Maria at San Salvador on 12 October 1492. Columbus believed that he had reached the East Indies and mistakenly called these people Indians. We know them today as the Lucayans. Columbus claimed the island and others in the Bahamas for his royal Spanish patrons, but not finding the gold and other riches he was seeking, he stayed for only two weeks before sailing towards Cuba.
> 
> The Spaniards never bothered to settle in the Bahamas, but the number of shipwrecks attest that their galleons frequently passed through the archipelago en route to and from the Caribbean, Florida, Bermuda, and their home ports. On Eleuthera the explorers dug a fresh-water well — at a spot now known as “Spanish Wells” — which was used to replenish the supplies of water on their ships before they began the long journey back to Europe with their cargoes of South American gold. As for the Lucayans, within 25 years all of them, perhaps some 30,000 people, were removed from the Bahamas to work — and die — in Spanish gold mines and on farms and pearl fisheries on Hispaniola (Haiti), Cuba, and elsewhere in the Caribbean.

The command ```grep -i``` with ```'pattern/words'``` and ```path``` same as the previous example except used on a diffrent file and word. Useful because it allows you to perform a case-insensitive search for a pattern or keyword within a file or set of files and if you are unsure of the exact case. 

##  ```grep -v``` ([source](https://www.cyberciti.biz/faq/howto-use-grep-command-in-linux-unix/))
- Example 1
> $ grep -v 'the' ./written_2/travel_guides/berlitz2/Bahamas-History.txt
> 
> A Brief History
> 
> Colonization and Piracy
> 
> The American Revolutionary War
> 
> Emancipation and Decline
> 
> Civil War Blockade Running
> 
> The 20th Century

The command ```grep -v``` with ```'pattern/words'``` and ```path``` uses the given pattern and invert match as it returns the lines within the file that doesn't contain the patten also pattern is exact case. 
- Example 2 
> $ grep -v 'e' ./written_2/travel_guides/berlitz2/Athens-WhereToGo.txt
> 
> Plaka and Anafiotika
> 
> Monastiráki and Thissio
> 
> From Omonia to Syntagma
> 
> Surrounding Syntagma
> 
> Excursions
> 
> Poros
> 
> Hydra
> 
> Corinth
> 
> Sounion

The command ```grep -v``` with ```'pattern/words'``` and ```path``` same as the previous example but used on a vowel. Useful because it allows you to exclude lines from a search result that match a specified pattern.
