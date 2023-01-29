# Places Around Me
## Aim:
To develop a website to display details about the places around my house.

## Design Steps:
### Step 1
Create a new django project and app

### Step 2: 
Add a new imagemap html file in templates and neede images in static folder and define it in settings.

### Step 3: 
Type ur image map code in the html with coordinates and target file to redirect on click

### Step 4: 
Define your components pages and create content in such a way that it gives information about place which is being clicked

### Step 5: 
Include pictures and contents for your subpages and map them using urls and views

## Code:
```
map.html:
<!DOCTYPE html>
<html>
    <head>
        <title>Marina Beach Image Map</title>
    </head>
    <body>
        <h1 align='center'>Map of marina beach</h1>
        <h2  align='center'>Address:</h2>
        <h3 align='center'>372J+4JP, South Ave, Kamaraj Nagar, Thiruvanmiyur, Chennai, Tamil Nadu 600041</h3>
        <img src = "/static/images/map.png" height="750" width="1800" align="center" usemap="#imgmap">
        <map name="imgmap">
           <area target="" alt="stadium" title="stadium" href="stadium.html" coords="413,514,389,462,399,406,425,387,449,370,482,367,529,372,565,416,565,476,528,523,470,540" shape="poly">
           <area target="" alt="presidency college" title="presidency college" href="presidency.html" coords="611,709,545,745,492,797,669,773,498,805,562,882,622,888,664,872,695,862,707,836,718,802,715,755,686,711,647,709,624,716" shape="poly">
           <area target="" alt="mgr memorial" title="mgr memorial" href="mgr.html" coords="1025,286,1020,304,1000,315,992,341,1008,357,1039,374,1065,374,1085,370,1119,349,1126,312,1093,289,1054,286" shape="poly">
           <area target="" alt="anna memorial" title="anna memorial" href="anna.html" coords="1056,157,1021,170,1012,207,1016,229,1026,251,1041,256,1065,260,1088,255,1108,251,1109,224,1106,198,1106,185,1087,162" shape="poly">
           <area target="" alt="madras university" title="madras university" href="university.html" coords="811,192,839,190,881,188,898,171,899,128,873,107,829,104,806,109,790,120,775,135,774,157,780,177,793,185" shape="poly">
        </map>
    </body>
    </html>

anna.html:
<!DOCTYPE html>
<html>
    <head>
        <title>Arignar Anna Memorial</title>
    </head>
    <body>
        <h1 align='center'>Arignar Anna Memorial</h1>
        <img src ="/static/images/anna.jpg"  height="500" width="1000" align="center" >
        <p>
           Anna Memorial, locally known as Anna Samadhi or as Anna Square, is a memorial structure built on the Marina beach in Chennai, India. It was built in memory of former Chief Minister of Tamil Nadu, C. N. Annadurai (1967–69), who was cremated here in 1969. The memorial is also the burial place of his protégé M. Karunanidhi. The memorial lies on the northern end of the Marina abutting the MGR Memorial, the burial place of Karunanidhi's archrivals, M. G. Ramachandran and J. Jayalalithaa. 
           In 1996–1998, during the reign of the DMK party, the memorial was remodelled at a cost of ₹ 27.5 million[1] and the entrance arch carried the design of the 'Rising Sun', the symbol of the DMK party. However, the design was removed after the opponent AIADMK party returned to power in May 2001.[2] The renovation resulted in the original tusk-shaped entrance arch giving way to a highly polished marble tiled structure, widened pathways, and building of ornamental octagonal mantapams. After the Indian Ocean tsunami struck the coastal parts of the state in December 2004, the memorial, along with other structures on the seashore, was affected. Subsequently, repair works were undertaken at a cost of ₹ 13.3 million.[1]

In 2012, the memorial was renovated at a cost of ₹ 12 million.[1] In 2018, when his protégé M. Karunanidhi, died, he was buried behind his mentor. A new memorial for Karunanidhi is being planned at a cost of ₹390 million rupees.
        </p>
    </body>

</html>

mgr.html:
<!DOCTYPE html>
<html>
    <head>
        <title>Dr.M.G.R Memorial</title>
    </head>
    <body>
        <h1 align='center'>Dr.M.G.R memorial</h1>
        <img src ="/static/images/mgr.jpg"  height="500" width="1000" align="center" >
        <p>
           The memorial was built in 1988 and inaugurated by V. N. Janaki Ramachandran, wife of M. G. Ramachandran, in May 1990.[3] The memorial was remodelled and the complex was laid with marble and opened in 1992 by J. Jayalalithaa who had become the chief minister of the state of Tamil Nadu in the previous year. When J. Jayalalithaa died on 5 December 2016, she was buried next to MGR. This structure was designed by architect K. Ramachandran, retired chief architect of PWD. Between 1996 and 1998, the mausoleum was again renovated at a cost of about ₹ 27.5 million. When the Indian Ocean tsunami struck the seafront in December 2004, the memorial was damaged. Repair works cost approximately ₹ 13.3 million.
           In 2012, the memorial was again renovated at a cost of ₹ 43 million, including ₹ 34 million for remodelling the facade and the surrounding wall.[5] This renovation included a new entrance with the AIADMK party's two-leaves symbol and Pegasus, the horse from Greek mythology, landscaping of the open area around the memorial using Korean grass, and the planting of exotic, decorative plants such as palmyra alpha, date palm, spider lily and adenium. Also included were a granite pathway shaped like a guitar, stainless steel handles around the memorial, a fountain in the middle, waterfall at the rear, decorative lamps, and an overhead tower with lights both at the entrance and on the arch.[1][6] Two pergolas 18 metres wide were also constructed, in addition to ramps for the physically challenged.[5]

The erection of the two-leaves insignia was opposed by the opposition DMK party.[7] A public interest petition was filed in the Madras High Court in October 2012 against the erection of the two-leaves insignia,[8] but was dismissed by the court.[9][10]
Jayalalithaa's burial site and memorial

In 2016, when his protégé J. Jayalalithaa died, she was buried behind her mentor, opposite to the memorial to her archrival, M. Karunanidhi. A new memorial was built for her at a cost of ₹500 million rupees. The Jayalalithaa Memorial or the Amma Memorial is shaped like a phoenix. The Construction Works of Jayalalithaa's memorial started on 7 May 2018.[11]

On 27 January 2021, The memorial of Jayalalithaa was inaugurated by then Chief Minister of Tamil Nadu Edappadi K. Palaniswami.
        </p>
    </body>

</html>

presidency.html:
<!DOCTYPE html>
<html>
    <head>
        <title>Presidency College</title>
    </head>
    <body>
        <h1 align='center'>Presidency college</h1>
        <img src ="/static/images/presidency.jpeg"  height="500" width="1000" align="center" >
        <p>
            Sir Thomas Munro asked for a Committee of Public Instruction to form in 1826. In 1836, the committee's duties changed to the "Committee of Native Education". The plans drawn up by the committee did not commend themselves to the Governor of Madras, Lord Elphinstone, who proposed nineteen resolutions that passed unanimously.[2]

Elphinstone chose E. B. Powell, a University of Cambridge Wrangler in mathematics, to be the first principal, and Powell accepted the post. He arrived in Mumbai (Bombay) on September 20, 1840, but did not reach Chennai (Madras) until 24 November. Meanwhile, the committee had invited Cooper from Hoogly College, Kolkata, to temporarily carry out the principal duties at a salary of Rs 400 per month. Cooper accepted the invitation and came to Chennai (Madras). He and his staff opened Presidency School, a preparatory school, in a rented building in Egmore known as Edinburgh Home, on 16 October 1840. Cooper remained in the primary school for only a few months. Soon after Powell's arrival, and before the high school department opened on 12 April 1841, he returned to Kolkata. The preparatory school shifted to Popham's Broadway in 1841.[2]

The schools grew into Presidency College. When the University of Madras was founded in 1857, Presidency College became affiliated with it.[2]

In 1870, the college moved to its present location in Kamaraj Salai, opposite Marina Beach.[3] 
        </p>
    </body>

</html>

stadium.html:
<!DOCTYPE html>
<html>
    <head>
        <title>M.A. Chidambaram Stadium</title>
    </head>
    <body>
        <h1 align='center'>M.A. Chidambaram Stadium</h1>
        <img src ="/static/images/stadium.jpeg"  height="500" width="1000" align="center" >
        <p>
            M. A. Chidambaram Stadium, commonly known as the Chepauk Stadium, is a cricket stadium in Chennai, Tamil Nadu, India.[3] Established in 1916, it is the second oldest cricket stadium in the country after Eden Gardens in Kolkata. Formerly known as Madras Cricket Club Ground, the stadium is named after M. A. Chidambaram Chettiar, former president of BCCI and Head of TNCA. It is the home ground of the Tamil Nadu cricket team and the Indian Premier League team Chennai Super Kings. Chepauk hosted its first Test match on 10 February 1934, the first Ranji Trophy match in 1936 and the Indian cricket team's first test victory in 1952 against England. The 1986 India-Australia match held at Chepauk was only the second ever Tied Test in the history of the game. 
        </p>
    </body>

</html>

university.html:
<!DOCTYPE html>
<html>
    <head>
        <title>Madras University</title>
    </head>
    <body>
        <h1 align='center'>Madras University</h1>
        <img src ="/static/images/university.jpeg"  height="500" width="1000" align="center" >
        <p>
            The University of Madras (informally known as Madras University) is a public state university in Chennai, Tamil Nadu, India.[2] Established in 1857, it is one of the oldest and among the most prestigious universities in India, incorporated by an act of the Legislative Council of India under the British government.[3]

It is a collegiate research university and has six campuses in the city: Chepauk, Marina, Guindy, Taramani, Maduravoyal and Chetpet. It offers more than 230 courses under 87 academic departments of post-graduate teaching and research grouped under 18 schools, covering diverse areas such as sciences, social sciences, humanities, management and medicine along with 121 affiliated colleges and 53 approved research institutions. The university houses national centres for advanced research in nanotechnology,[4] photonics[5] and neurotoxicity.[6] In addition, it has three Centres of Advanced Study (CAS) in biophysics,[7] botany[8] and the Ramanujan Institute for Advanced Study in Mathematics.[9]

University of Madras is the alma mater of five presidents of India, including A. P. J. Abdul Kalam; two Indian physics Nobel laureates, CV Raman and Subrahmanyan Chandrasekhar; several notable mathematicians including Srinivasa Ramanujan; Abel Prize winner S. R. Srinivasa Varadhan; and Turing Award winner Raj Reddy among others.[10]

The National Assessment and Accreditation Council has conferred 'five star' accreditation to the university in the first cycle, and subsequently with its highest 'A' grade.[11] The University of Madras has been given the status of 'university with potential for excellence (UPE)' by the University Grants Commission.[12] Madras University is also recognized among the 18 universities in India having the 'Centre with Potential for Excellence in Particular Area (CPEPA)' with a focus on drug development and climate change.[13] 
        </p>
    </body>

</html>
```
## Output:
![output](/beach.png)
![output](/stadium.png)
![output](/memorial.png)
![output](/mgr.png)
![output](/anna.png)
![output](/madras.png)
## Result:
Thus a website is developed to display details about the places around my house
