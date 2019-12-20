# Morse-Code-Encryter-Decrypter
Morse code is a method of transmitting text information as a series of on-off tones, lights, or clicks that can be directly understood by a skilled listener or observer without special equipment. It is named for Samuel F. B. Morse, an inventor of the telegraph.

## Algorithm

The algorithm is very simple. Every character in the English language is substituted by a series of ‘dots’ and ‘dashes’ or sometimes just singular ‘dot’ or ‘dash’ and vice versa.
Please refer this wikipedia image for details.

## Encryption
In case of encryption we extract each character (if not a space) from a word one at a time and match it with its corresponding morse code stored in whichever data structure we have chosen(if you are coding in python, dictionaries can turn out to be very useful in this case)
Store the morse code in a variable which will contain our encoded string and then we add a space to our string which will contain the result.
While encoding in morse code we need to add 1 space between every character and 2 consecutive spaces between every word.

## Decryption
In case of decryption, we start by adding a space at the end of the string to be decoded (this will be explained later).
Now we keep extracting characters from the string till we are not getting any space.
As soon as we get a space we look up the corresponding English language character to the extracted sequence of characters 
(or our morse code) and add it to a variable which will store the result.
Remember keeping track of the space is the most important part of this decryption process. As soon as we get 2 consecutive spaces we will add another space to our variable containing the decoded string.
The last space at the end of the string will help us identify the last sequence of morse code characters 
(since a space acts as a check for extracting characters and start decoding them).

### International Morse Code Letters - 

#### A	= · –                                     
#### B	= – · · ·
#### C	= – · – ·
#### D	= – · ·
#### E	= ·
#### F	= · · – ·
#### G	= – – ·
#### H	= · · · ·
#### I	= · ·
#### J	= · – – –
#### K	= – · –
#### L	= · – · ·
#### M	= – –
#### N	= – ·
#### O	= – – –
#### P = · – – ·
#### Q	= – – · –
#### R	= · – ·
#### S	= · · ·
#### T	= –
#### U	= · · –
#### V	= · · · –
#### W	= · – –
#### X	= – · · –
#### Y	= – · – –
#### Z	= – – · ·
### International Morse Code Numbers and Punctuation - 

#### 1	· – – – –
#### 2	· · – – –
#### 3	· · · – –
#### 4	· · · · –
#### 5	· · · · ·
#### 6	– · · · ·
#### 7	– – · · ·
#### 8	– – – · ·
#### 9	– – – – ·
#### 0	– – – – –
#### Period	· – · – · –
#### Comma	– – · · – –
