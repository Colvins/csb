# CSB
#### What is CSB?
CSB or Community Supreme Bot is a project that has been in development for nearly a year now. Previously known as FESBSC, CSB is a completely free open source bot to cop clothing items from Supreme. Evidently, a market for Supreme bots has developed within the Supreme Community. This market has become saturated with bots that seldom work at prices exceeding hundreds of dollars. The CSB project is an attempt to remove these huge paywalls, allowing all members of the Supreme community a fair chance in copping the items they want without any extra burdens on their wallet. This being said, CSB is still in development and success will never be 100% guaranteed. However, we are constantly working on the bot in order to raise the success rate with ambitious yet capable plans for the future involving new tech which has never been utilised within this field. Currently CSB is being developed by a two man team: me – Tom, also known as HA6Bots and Daniel commonly referred to as Danielyc on forums. We have been working very hard throughout the summer to create a stable and functioning bot in preparation for the fall/winter season 2018. This being said, we are proud to release CSB V3.0. Again, we emphasise that the bot is a work in progress and success is not guaranteed. By downloading and using this tool, you as an individual are responsible for the output whether you successfully purchase your item or not. We accept no responsibility for any mishaps that may occur.
#### FAQ
#### Are my payment details safe?
Yes. The bot itself (the python scripts) does not connect to any servers. The tool itself is completely client side, payment details (if chosen) are kept on your personal device in an encrypted .cnf file located within your CSB folder directory. The user has the option of saving payment and billing details when prompted to. Again, I repeat this is stored in an encrypted .cnf file which is only accessible via your personal password. Alternatively, the user does not have to save these details and can use the program as normal. The source code is on GitHub at https://github.com/danielyc/csb and can be analysed for complete transparency.
#### How was CSB made?
CSB is made with python. We utilise several libraries in order to make the bot functional. Selenium is used with chromedriver to replicate user interactions with the Supreme website. We use PyQt5 for the UIs. We are planning to replace Selenium and the chromedriver in the near future with our own custom library which will utilise Image recognition technology.
#### Why is CSB free?
There are several reasons why the CSB project is free:
1. We want to send a message to the companies that have been exploiting the Supreme Community for years with extortionate fees for outdated bots that barely work: This is not a productive use of technology and is a business model that is unethical and out-right shady. We want to show that the prices that have been charged by these companies and individuals are completely artificial – if two people can create a bot at no other expense then a few hours a day, why are single use bots going for $200+?
2. The bot is still in development. The bot will always be in development. This is the nature of bots – things keep getting updated, Supreme will always push out new changes to their website, so we will need to make sure the bot is responsive to all these changes. Thus there will always be an element or risk that the bot will not work. However small this risk might be, it will always exist and therefore there is always a chance it will not work. Even if there is a 1% chance that the bot will be unsuccessful, this means that one out of a hundred people would have wasted their money. The only solution to this issue is to keep the bot free.
3. We like Supreme. The bot is a gift to the Supreme Community and gifts are free.
#### Will development be sustainable?
Currently CSB is being developed by two people – me (Tom) and Daniel. I will be working full time very soon while Daniel will start university in early September. However this will not stop us from continuing development on the bot. Last year we both had school and still managed to push out the first two versions of the bot. At the moment, apart from time – monetary costs are low. We are planning to further the project with some servers and a website in the near future. We will always keep the bot free for everyone to use. We may at some point look into different avenues for monetization such as advertisements but we will never introduce any paywalls that undermine the functionality and idea behind CSB.
#### How can I support the CSB project?
Like mentioned before CSB will and always will be free. We will never ask for any money as CSB is a gift to the community. You can support us by telling your friends/fellow Supreme users about CSB and help spread the word that a free and trustworthy bot exists. If you really want to support the project you can donate to our PayPal at https://www.paypal.me/supportcsb . We also have a Bitcoin and Ethereum wallet: BTC `32U1WNf47UXcmDuMoJ7vezKd7UGRXmqPFP` ETH `0xd445FC2b12B15A0FcA52153a75956bAb843bD03a`. We appreciate any donations of any amount. We will also add your name to the donor list in the credits section of the bot unless you say otherwise. The money will help finance any costs involved with the bot such as domains, websites, servers etc. 
#### Will CSB completely automated? Is there anything I have to do manually?
Currently for CSB V3.0 we have not reached full automation. While the bot will automatically find and add the item to the basket as well as filling out all the billing/shipping details, a google Captcha will appear at the end. This is the only process the user manually has to complete. Once the Captcha is completed the purchase will be completed. We are working hard to bypass the Captcha and already have some prototype concepts in production. Please read the instructions located at the bottom of this document for more information. 
#### What is the licencing for CSB?
CSB operates under GNU AGPLv3. You are free to use the tool however you want. As long as it is compliant with the licence.
#### What OS (Operating Systems) is CSB compatible with?
As of now, windows 7 through 10 and MacOS
#### Can I help with the production of CSB?
At the moment we are not looking for any new members to join the team. Currently, the project is not big enough for multiple people to work on it without causing greater inconveniences. This being said, you can still help us by emailing us crash reports to info@csb.center or open bugreports on the github page.
#### How can I get in contact with the CSB team?
You can get in contact with us by emailing info@csb.center.
# How to use CSB
1. Download the CSB binary or the zipfile from the website
- http://csb.center
2. Open the downloaded zip file and drag and drop the containing folder ‘CSB’ onto your desktop or where you would like to store the bot.
3. Download chromedriver from http://chromedriver.chromium.org/downloads, make sure you download the right version if you are using Mac or Windows. Place chromedriver in your CSB folder.
4. Ensure that google chrome is downloaded and installed on your device. You can download chrome from https://www.google.com/chrome/.
5. If Chrome it not installed into the default location, make a text file named 'chromepath.txt' in the CSB folder with the path to the Chrome executable
6. If you have downloaded the binary version of CSB, then you are done now with the installation and you can skip to step 9. If you have downloaded the source files then read along.
7. Make sure you have installed the latest version of python for your operating system.
8. Install the required python libraries using `pip install -r requirements.txt`.
9. Run **main.py**, **main.exe** or on Mac open a terminal window and drag **main** into it and press enter. If there is an update available then there will be a popup.
10. Choose the region you are located in. If you live in Canada pick “US”. The “ASIA” option refers to Japan only as this is the only place where Supreme ships to within Asia. Then click on “New config”. If you already have a configuration file then select it from the dropdown menu and input the password.
11. If you chose to make a new configuration file a window will show where you can enter all of your payment and shipping details.
12. This is where you enter all of the shipping and billing details. You have the option of saving this info in a local .cnf file which will be stored within the same directory. This information is encrypted and can only be decrypted with your personal password. If you would like to save this information for multiple uses, enter a password within the password field and also a save name. The .cnf file will be named whatever you enter in the save name field. Click the button “Save config” to save this information or click “Continue” to proceed unsaved.
13. Now the next window will popup which is used to input the items to cop.
14. Go to https://www.supremecommunity.com/season and search for the latest droplist. Determine what item(s) you want to cop. Please note you can only purchase one of any item. If you would like to buy the **Water Arc Hooded Sweatshirt** for example then you have to take the following steps:
- Select the correct category from the dropdown menu, in this case **sweatshirts**
- Next is the most important bit. You need to split up the name of the item into keywords. This is easy: separate every word with a comma. For example: **Water Arc Hooded Sweatshirt** should be entered into the keywords input box as: **Water,Arc,Hooded,Sweatshirt**. For the item **Supreme®/Lucano® Step Ladder** enter the keywords as **Supreme®/Lucano®,Step,Ladder**. Replace any spaces with a comma.
- Next identify the colour input box. This refers to the colour or model of the item you want. This is the tricky bit because these models/colours are not given on the Supreme Community website. So your best bet is to guess what the model/colour will be. For the above item “Water Arc Hooded Sweatshirt”, the image suggests there will be a white version of the item. So enter “White” into the colour input box. This input box is also used for the model version for skate boards.
- Now choose the size of the item you want. **NOTE** if the size chosen is not available the bot will choose the first available size for the item. Therefore, choose a size which you think the item will be available in. **TIP** it is rare that Supreme releases items in small. If you want the smallest version but are unsure whether or not it will be available pick the option “First available” as this will be the smallest possible size. The most common sizes are  “Medium” and “Large”.
- Now select the time of the drop in your native time. In the UK this is 11am, so I will choose the 11:00 option. When the time on your device reaches the time you have selected for the drop the bot will start working. So make sure the time on your computer is accurate and adjusted to an accurate time. You can get the exact time at https://time.is 
- Now press **Add item** to add it to the list the bot will attempt to cop.
15. Strict Item Selection: Strict Item Selection is a feature that is supposed to prevent wrong items being selected by the bot. The feature causes the bot to make sure there is a 100% match with the keywords and colour specified. If the Supreme site does not update before the bot executes, the bot will continually refresh the page till the listing becomes available. Therefore we recommend to keep strict item selection on within the options menu. The downside to this search option is that if the information in the keywords and colour input are not 100% correct, the bot will not be able to find the listing and will not complete the purchase – hence continually refresh the page indefinitely. If you choose to unselect Strict Item Selection, the bot will choose the item with the closest match according to keywords and colour. If Supreme has not updated in time, and the bot executes before the page has been updated the bot will choose the closest option which could be completely different from what you wanted. Thus we recommend you keep Strict Item Selection selected.
16. Press **GO!** when you have chosen all the items you want. This will begin chromedriver which will open a blank window.
17. **IMPORTANT!** Do not close this window, do not minimize it, and do not use it to browse the internet. When the selected drop time comes, the browser will automatically open the Supreme website and begin finding your items and filling in information. A few minutes before the drop ensure that you close all other RAM/Broadband intensive programs on your computer. Full screen the chromedriver browser and stay alert. Once the time comes, the bot will load Supreme and start doing its magic. It will open the Supreme page with the right category first then find and decide which item matches the keywords, pick the size, add it to the basket and enter the billing and payment details.
18. **STAY AT YOUR COMPUTER SCREEN!** In CSB V3.0 it is likely a google captcha will pop out when confirming the purchase. We are working on new methods to bypass the captcha, however we have not had enough time to implement them for 3.0 so at the moment the captcha must be entered manually. This will only take a few seconds, so please do not leave your computer completely unattended. **NOTE**: the PayPal checkout will not automatically enter your email and password so be prepared to copy and paste them in when it appears.
19. After completing the Captcha, assuming your pay details and billing information is correct, you should be finished. Please let us know how the experience was by emailing us at info@csb.center


If CSB worked as intended or you want to support the project, you can donate at https://www.paypal.me/supportcsb. Any amount is appreciated and we will add your name if you wish to the donor list which will be included on a later version
Thanks!
-HA6Bots and Danielyc