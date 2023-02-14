## Lab 04

- Name:anuja alluri
- Email: alluri.17@wright.edu

## Part 1 Answers

1. `grep -E '^[0-9]{3}-[0-9]{3}-[0-9]{4} [x|X][0-9]{4}' grepdata.txt`
2. `grep -E '..+?(\CA|ca) [0-9]*-*[0-9]*' grepdata.txt`
3. `grep -E "..+?@.+?" grepdata.txt`
4. `grep -E '[A-Z][a-z][a-z]\. ..+?[0-9]{3}' grepdata.txt`

## Part 2 Answers

1. `sed -i 's/<\w\w>$//g' sedfile.html`
2. `sed -i 's/<li>/-/g' sedfile.html`
3. `sed -i 's/<h1>/#/g' sedfile.html`
4. `sed -i 's/<h2>/##/g' sedfile.html`
5. `sed -i 's/<html>//g' sedfile.html , sed -i 's/<ul>//g' sedfile.html`
6. `sed -i 's/Batches/Matches/' sedfile.html`

## Part 3 Answers

1. awk '$1~/Bil/ {print $1}' records.tx
2. awk '$4~/42/ {print $3}' records.txt 
3. awk '$3~/wright.edu/ {print $2",",$1": "$3 }' records.txt
4. awk '$3~/wright.edu/ &&$6~/1234/{print $2 " favorite number is:", $4}' records.txt
5. awk '{ gsub($6,"N0T@PL@!NP@$$W0RD",$6); print $0}' records.txt > updaterecords.txt
