# Hash Extender by Ron Bowes <ron@skullsecurity.net>

This will be a blog post on http://www.skullsecurity.org/. For now, it's a README file.

## Intro

**You can grab the hash_extender tool on [Github](https://github.com/iagox86/hash_extender)!**

Awhile back, my friend [mogigoma](http://twitter.com/mogigoma) and I were doing a capture-the-flag contest at [https://stripe-ctf.com](https://stripe-ctf.com). One of the levels of the contest required us to perform a hash length extension attack. I had never even heard of the attack at the time, and after some reading I realized that not only is it a super cool (and conceptually easy!) attack to perform, there is also a total lack of good tools for performing said attack!  After hours of adding the wrong number of null bytes or incorrectly adding length values, I vowed to write a tool to make this easy for myself and anybody else who's trying to do it. So, after a couple weeks of work, here it is!

Now I'm gonna release the tool, and hope I didn't totally miss a good tool that does the same thing! It's called `hash_extender`, and implements a length extension attack against every algorithm I could think of:

- MD4
- MD5
- RIPEMD-160
- SHA-0
- SHA-1
- SHA-256
- SHA-512
- WHIRLPOOL

I'm more than happy to extend this to cover other hashing algorithms as well, provided they are "vulnerable" to this attack -- MD2, SHA-224, and SHA-384 are not. Please contact me if you have other candidates and I'll add them ASAP!
