<style>
/* The dropdown container */
.dropdown {
  float: left;
  overflow: hidden;
}
/* Dropdown button */
.dropdown .dropbtn {
  font-size: 16px;
  border: none;
  outline: none;
  color: white;
  padding: 14px 16px;
  background-color: inherit;
  font-family: inherit; /* Important for vertical align on mobile phones */
  margin: 0; /* Important for vertical align on mobile phones */
}
/* Add a red background color to navbar links on hover */
.navbar a:hover, .dropdown:hover .dropbtn {
    background-color: aliceblue;
    color: teal;
  }
  /* Dropdown content (hidden by default) */
.dropdown-content {
  display: none;
  position: absolute;
  background-color: teal;
  min-width: 160px;
  box-shadow: 0px 8px 16px 0px rgba(0,0,0,0.2);
  z-index: 1;
}
/* Links inside the dropdown */
.dropdown-content a {
  float: none;
  color: aliceblue;
  padding: 12px 16px;
  text-decoration: none;
  display: block;
  text-align: left;
}
/* Add a grey background color to dropdown links on hover */
.dropdown-content a:hover {
  background-color: #ddd;
}
/* Show the dropdown menu on hover */
.dropdown:hover .dropdown-content {
  display: block;
}
</style>
<nav class="w3-container w3-teal w3-center w3-margin-top">
    <div class="dropdown">
        <button class="dropbtn">Projects
          <i class="fa fa-caret-down"></i>
        </button>
        <div class="dropdown-content">
          <a href="https://russc-xer0n3.github.io/NetPCaC">NetPCaC</a>
          <a href="https://russc-xer0n3.github.io/LANDROVER">LANDROVER</a>
          <a href="https://russc-xer0n3.github.io/MAC">MAC Address</a>
          <a href="https://russc-xer0n3.github.io/SCRUD">SCRUD</a>
          <a href="https://russc-xer0n3.github.io/Remove">Code Syntax Removal</a>
          <a href="https://russc-xer0n3.github.io/PassGen">PassGen</a>
          <a href="https://russc-xer0n3.github.io/C_Shapes">C Programming Shap`es</a>
          <a href="https://russc-xer0n3.github.io/Shapes---python">Python Shapes and space</a>
          <a href="https://russc-xer0n3.github.io/The-old-Fusion-Repository">Fusion?</a>
          <a href="https://russc-xer0n3.github.io/The-Russian-Wedding-Rings">The Russian Wedding Rings</a>
          <a href="https://russc-xer0n3.github.io/QBit-and-GParticulates">QBit and GParticulates</a>
          <a href="https://russc-xer0n3.github.io/Thyme-old">Thyme</a>
          <a href="https://russc-xer0n3.github.io/IP-Port">IP and Ports</a>
          <a href="https://russc-xer0n3.github.io/Xer0n3">Xer0n3</a>
          <a href="https://russc-xer0n3.github.io/ScrambledEggs">ScrambledEggs</a>
          <a href="https://russc-xer0n3.github.io/Py">Python Code</a>
        </div>
    </div>
    <br>
      <a href="https://www.facebook.com/profile.php?id=100075972987666"><i class="fa fa-facebook-official w3-hover-opacity"></i></a>
      <a href="https://www.instagram.com/russellclarke821"><i class="fa fa-instagram w3-hover-opacity"></i></a>
      <a href="https://www.pinterest.co.uk/russellclarke821/"><i class="fa fa-pinterest-p w3-hover-opacity"></i></a>
      <a href="https://twitter.com/Developing821"><i class="fa fa-twitter w3-hover-opacity"></i></a>
      <a href="https://www.linkedin.com/in/russell-clarke-09a1a5238"></a><i class="fa fa-linkedin w3-hover-opacity"></i>
      <a href="https://russc-xer0n3.github.io">My CV and additionsl information</a>
    <br>
</nav>
# IP Port
## Simply taking a look and rolling autogen loops

### hostname
The purpose of this script is to systematically run through a 36 character combination and produce every possible outcome of that sequence to autogenerate quite a large portion of potential hostnames. It is not dissimilar in nature to rainbow tables, just a lot slower.

```
#!/usr/bin/env python

# A simple name generator includes numerical values
# @author Russell Clarke aka Rusher SD200984
# @version 1.0
# @Created 22.12.2018
# @Listening to : Elephant Ride - State of Bengal

for a in range(36):
	a1 = '%x' % a
    for b in range(36):
    	a2 = '%x' % b
        for c in range(36):
        	a3 = '%x' % c
        	for d in range(36):
				a14 = '%x' % a
				for e in range(36):
					a5 = '%x' % e
					for f in range(36):
						a6 = '%x' % f
						for g in range(36):
							a7 = '%x' % g
							for h in range(36):
								a8 = '%x' % h
								for i in range(36):
									a9 = '%x' % i
									for j in range(36):
										a10 = '%x' % j
										for k in range(36):
											a11 = '%x' % k
											for l in range(36):
												a12 = '%x' % l
												for m in range(36):
													a13 = '%x' % m
            										print('.' + a13 + a12 + a11 + a10 + a9 + a8 + a7 + a6 + a5 + a4 + a3 + a2 + a1)
            										
exit(0)
```

## A brick wall
### Generating IPv6 addresses
I got quite close with this one however there are a few caveates which have to be addressed, they are;

- Formatting
- Quantity of nested loops permitted in Python
- Trying to speed up the generation process for 'o(log)n' notation

### Some success
```
#! /usr/bin/env python

# Simple to increment some values.
# @author Russell Clarke 0ka Rusher SD200984
# @version 1.5
# @Created 21.12.2018
# @Listening to Linkin Park et.al
# There are too many nested blocks and so I must rethink the logic proof of concept is in the mac_daddy.py and ip.py

#for a in range(16):
#    z = '%x' % a
#    x = '%x' % a
#    y = '%x' % a
#    w = '%x' % a
#    for b in range(16):
#        v = '%x' % b
#        u = '%x' % b
#        t = '%x' % b
#        s = '%x' % b
#        for c in range(16):
#            r = '%x' % c
#            q = '%x' % c
#            p = '%x' % c
#            o = '%x' % c
#            for d in range(16):
#                n = '%x' % d
#                m = '%x' % d
#                l = '%x' % d
#                k = '%x' % d
#                col = ':'
#                print(z + y + x + w + col + v + u + t + s + col + r + q + p + o + col + n + m + l + k + col + j + i + h + g + col + f + e + d + c + col + b + a + z #+ y + col + x + w + v + u)

for a in range(16):
	z = '%x' % a
	for b in range(16):
		y = '%x' % b
		for c in range(16):
			x = '%x' % c
			for d in range(16):
				w = '%x' % d
				for e in range(16):
					v = '%x' % e
					for f in range(16):
						u = '%x' % f
						for g in range(16):
							t = '%x' % g
							for h in range(16):
								s = '%x' % h
								for i in range(16):
									r = '%x' % i
									for j in range(16):
										q = '%x' % j
										for k in range(16):
											p = '%x' % k
											for l in range(16):
												o = '%x' % l
												for m in range(16):
													n = '%x' % m
													for n in range(16):
														m = '%x' % n
														for o in range(16):
															l = '%x' % o
															for p in range(16):
																k = '%x' % p
																for q in range(16):
																	j = '%x' % q
																	for r in range(16):
																		i = '%x' % r
																		for s in range(16):
																			h = '%x' % s
																			for t in range(16):
																				g = '%x' % t
																				for u in range(16):
																					f = '%x' % u
																					for v in range(16):
																						e = '%x' % v
																						for w in range(16):
																							d = '%x' % w
																							for x in range(16):
																								c = '%x' % x
																								for y in range(16):
																									b = '%x' % y
																									for z in range(16):
																										a = '%x' % z
																										for za in range(16):
																											ab = '%x' % za
																											for zb in range(16):
																												ac = '%x' % zb
																												for zc in range(16):
																													ad = '%x' % zc
																													for zd in range(16):
																														ae = '%x' % zd
																														for ze in range(16):
																															af = '%x' % ze
																															for zf in range(16):
																																ag = '%x' % zf
																																col = ':'
																																print(ag + af + ae + ad + col + ac + ab + a + b + c + col + d + e + f + col + g + h + i + j + col + k + l + m + n + col + o + p + q + r + col + s + t + u + v + col + w + x + y + z)


exit(0)
```

### However
There was the issue of too many nested loops although, syntactically, the code is correct and theoretically does work with the correct format and so a second attempt is on the way;

## IP6v2 
### UNFINISHED
```
#! /usr/bin/env python

# Simple to increment some values.
# @author Russell Clarke 0ka Rusher SD200984
# @version 1.5
# @Created 21.12.2018
# @Listening to Linkin Park et.al
# There are too many nested blocks and so I must rethink the logic proof of concept is in the mac_daddy.py and ip.py


a1 = '%x' % a
a2 = '%x' % b
a3 = '%x' % c
a4 = '%x' % d
#a5 = '%x' % 
#a6 = '%x' % 
#a7 = '%x' % 
#a8 = '%x' % 
#a9 = '%x' % 
#a10 = '%x' % 
#a11 = '%x' % 
#a12 = '%x' % 
#a13 = '%x' % 
#a14 = '%x' % 
#a15 = '%x' % 
#a16 = '%x' % 
#a17 = '%x' % 
#a18 = '%x' % 
#a19 = '%x' % 
#a20 = '%x' % 
#a21 = '%x' % 
#a22 = '%x' % 
#a23 = '%x' % 
#a24 = '%x' % 
#a25 = '%x' % 
#a26 = '%x' % 
#a27 = '%x' % 
#a28 = '%x' % 
#a29 = '%x' % 
#a30 = '%x' % 
#a31 = '%x' % 
#a32 = '%x' % 
se = ':'

for a in range(16):
	a1
    for b in range(16):
    	a2
        for c in range(16):
        	a3
            for d in range(16):
            	a4
                print(a4 + a3 + a2 + a1 + se)

exit(0)
```

Possibly, there will be 4 for loops maybe 5 or 6 to facilitate each 16bit portion of the address and concatinate them later on in the code.
<head>
    <meta content="text/html; charset=utf-8" http-equiv="Content-Type">
    <meta charset="UTF-8">
    <meta name="description" content="Projects and Portfolio">
    <meta name="keywords" content="HTML, CSS, JavaScript, PHP, MySQLi, Python, Java, C, C++, C#, Time, Shapes">
    <meta name="author" content="Russell Clarke">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <link rel="stylesheet" href="https://www.w3schools.com/w3css/4/w3.css">
    <link rel="stylesheet" href="https://fonts.googleapis.com/css?family=Roboto">
    <link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/4.7.0/css/font-awesome.min.css">
</head>
<footer class="w3-container w3-teal w3-center w3-margin-top">
  <p>Find me on social media.</p>
  <a href="https://www.facebook.com/profile.php?id=100075972987666"><i class="fa fa-facebook-official w3-hover-opacity"></i></a>
  <a href="https://www.instagram.com/russellclarke821"><i class="fa fa-instagram w3-hover-opacity"></i></a>
  <a href="https://www.pinterest.co.uk/russellclarke821/"><i class="fa fa-pinterest-p w3-hover-opacity"></i></a>
  <a href="https://twitter.com/Developing821"><i class="fa fa-twitter w3-hover-opacity"></i></a>
  <a href="https://www.linkedin.com/in/russell-clarke-09a1a5238"></a><i class="fa fa-linkedin w3-hover-opacity"></i>
  <p>Powered by <a href="https://www.w3schools.com/w3css/default.asp" target="_blank">w3.css</a></p>
</footer>
