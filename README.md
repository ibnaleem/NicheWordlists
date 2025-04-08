# NicheWordlists
A curated collection of unique and niche wordlists, including fruits, foods, countries, and more.

# Why Should I Use This?
> *Occam's razor suggests that when faced with multiple explanations for a phenomenon, the simplest explanation is usually the best.*

Passwords are (usually) a combination of words. The more combinations, the more complex. Arbitrarily cracking hashes with large wordlists instead of doing reconnaissance on the target hash(es) is bad strategy. 

Hashcat’s Combinator Attack (`-a 1`) is probably the best attack mode for successfully cracking hashes. The problem is there aren’t many wordlists that allow us to create meaningful combinations. 

For example, rockyou.txt contains the word `“letmein”`,and if we wanted to generate a candidate like `“blueberrycucumber”`, Hashcat may generate a candidate like `“blueberryletmein”` which is completely useless computationally. 

Instead, if we have a wordlist of fruits, another wordlist of vegetables, and do a Combinator Attack on these, we can generate much useful candidates without overly stressing our GPU. Additionally, Combinator Attacks are obsolete when large wordlists are used simply because the time it takes to create pairings can be used for intelligently crafting wordlists that could crack the password much quicker. 

That’s why this repository was created: a one place for specific wordlists (that are updated by the community) for your Combinator Attacks. Find whatever is useful, or add your own by contributing. 