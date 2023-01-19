# Operate First Community Cloud Meet Up
## S02E04 - 2022-11-29 - 11am ET
### The 5h Open Paradigm

Thorsten    00:00:03    Hello everybody. Welcome to our biweekly Operate First Community Cloud Meetup, and it's, again, Tuesday. It's again, 11:00 AM Eastern Time slash New York. Uh, we are recording this meeting to give everybody a chance to follow. You can find our privacy policies at OP one slash privacy policy. This Meetup is held under the Open Info Foundation Code of Conduct, which you can find at OP one slash Community code of Conduct. I will put this link, this links also in the check. You can look up everything about this meeting on the page you're just seeing here, which is OP one slash Meetup. And this Meetup is a gathering point for project services, lessons learned, help needed ideas on and around the Operate First idea in general, and the operate First Community cloud in particular. Uh, this meeting can be as interactive as needed. So we call it the Hands-on meeting if you want to. And I'm more than happy that Felix, I'm from the Sovereign Cloud Stack, uh, is presenting today. His, um, the fifth open paradigm of yeah, the fifth open paradigm, right? That's the thing. And, um, if you want to see him and or me in live, you can join the Foster 2023 in February, but we get to this later. I will now hand over to Felix and  
Thorsten    00:01:28    Go on  
Felix    00:01:29    <laugh>. Thanks a lot for this. I'm  
Felix    00:01:42    Sorry. So you should now see, uh, my presenters or the slides, not the presenters. You, hi. So I'm, uh, Felix, um, and, uh, invited me to, um, talk about something that, uh, we refer to as the fifth open. Um, and that's, uh, open operations. And, um, just, uh, couple words about, if I say we, um, Torson already said, uh, that I'm Felix from the Sovereign Cloud Stack Project. And, uh, the, uh, this will be actually, I'm, I will keep the advertisement very, very short. But, um, the Sovereign Cloud Stack Project is a project, um, that's hosted by the Open Source Business Alliance. The Open Source Business Alliance is in nonprofit organization in Germany that advocates for open source on, uh, political level. And, um, since, uh, two years ago, we actually have this project, which is funded by the Federal Ministry of Climate, of, of, of, uh, federal ministry, of Foreign of Foreign Affairs and Climate Action, I think.  
Felix    00:02:55    And, um, basically, um, we are running this project until the end of September 24. And, um, within the Sovereign Cloud Stack Project, we, um, have three pillars. And, uh, one pillar is that we define standards on how cloud environment on a container level in a federal situation. So they, federal bill should be designed, and basically we define a standard, and we back those standards by offering in the reference implementation on the infrastructure service level. That's based on opens Stack, and, uh, on the container level that's going to be cluster api. And basically, we define the standards and how to orchestrate the, uh, the cluster management so that basically you can move your infrastructure as code from one CSP to another, and if they're CS compliant, every single adjust work. And that way you can also, with the identities, you can actually have true multi-cloud. The idea behind this, that by that you actually create an environment where you are not dependent on the single vendor.  
Felix    00:04:02    And instead, um, we create a lot of innovation. And the research pillar that we actually have is what we call open operations. And, um, within the SCS project, we actually foster this, uh, open operations among the CSP that we work with. So that, uh, not every CSP as a silo works for themselves, but, uh, we act as a strong community. And that's basically what I'm going to elaborate on the next, uh, 25 minutes. Um, I'm not sure how you usually do that. I check with Toon if you have questions. We are not, uh, a gigantic group. If you have questions, feel free to raise your arm, I think to then moderated it. Um, we don't have to wait until the end to do a proper KU a session. We can just, uh, do that in between just how you feel. Uh, also at the end, I'm also available longer than just, uh, till 1130, so we can do that.  
Felix    00:04:58    So where do we come from? So, um, maybe some of you know that, uh, the Bazaar and Cathedral, um, if we look over the last, uh, 40 years, uh, in the IT industry, especially in the Oak Source movement, uh, we've, we've basically achieved a lot. Um, I just prepared actually a talk, um, for another location, uh, where I was collaborating on, on the open source development of the last 40 years. And basically it's clear that, uh, we won the game. So open source is a game changer. Um, everybody has acknowledged that the overall amount of pay or of workloads in any cloud environment are based on opensource, not only the workloads, but also all the stuff running below. It is basically without opensource, not, not possible. So I would say we actually won that game and, uh, from, from that viewpoint, our life should look like that.  
Felix    00:05:58    Um, nice Sun downer, free sheep running around eating grass. And, um, if we actually look at, uh, at some of the things that make this possible, it's, for example, um, the, um, fantastic four that originate from the, uh, open infra foundation, but there that are actually, um, present in a lot of communities, um, the, uh, open source, open design, open development, as well as the open community. And, um, the open infra embraces that. Um, being a somebody who works a lot in the open sector nowadays, um, the open foundation, of course, is, uh, very close to me. But, um, if, uh, if we look at that, we, we, we have the community, we have the development that works closely together. But, um, if we actually shift our view a bit away from, from the pure development side of things, and, uh, actually look a bit more onto the what do we do with the, with the source code, one that has been developed and, uh, at all the CSPs that actually operate all this stuff, um, life often looks, uh, a bit more like that.  
Felix    00:07:15    So, um, that's, uh, bit of the shock effect now. But, um, and, um, the, the IT landscape and, um, basically when, when I started in, uh, 97, uh, I founded a small ip and back then running infrastructure and things like mail servers using server and all that was, uh, a completely different item from today's world. So, um, so if you actually look at, uh, modern distributed dynamic infrastructure, it actually, uh, is, is really, um, a different kind of beast. And, um, so complexity keeps rising. Um, you need a lot of skill sets. You need a very broad skill set among, among your engineers. And, um, what, uh, what we actually see is that it's, it's time to, to take the patterns that we've actually used the last, uh, 40, 30 years in, in open source development to actually move that to the, to the operations side of things.  
Felix    00:08:24    And there are already a few, few movements on the way. So, um, if you, if you look at all the, all the DevOps items that, uh, have happened, um, since its initial first meeting in, in Belgium many years ago, and, uh, also the, the whole site reliability movement. So there, there is definitely a movement into the right part. And what, um, what we, um, in the Sovereign cloud tech project, when, when we wanted to talk about the subject at the summit, uh, last summer was, uh, we thought, okay, why maybe it's time to actually amend before opens the fifth open, um, open operations. And, um, the first thing, um, that basically came to mind is when, when we talk about open operations is that, um, one thing that we, we wanted to spark since we work with a lot of CCP is to make, um, certain aspects of the cloud environment of the CCP that we work with more transparent.  
Felix    00:09:30    And, um, what, uh, what we actually have is the, the tool that's called, um, open house monitor. So each CSP that, uh, we work with and is active in our community, we actually, um, hook up to the, to the open house monitor. And the open house monitor basically continuously over, um, the, the whole time spas machines, checks, whether they're reachable or not, and basically records each and every hour. And, um, the idea is, um, not from a pure monitoring aspect, but also to actually make this data available, um, to, to the, to everyone else and to the public. And, um, we, and if we actually talk, talk to cease piece about that is that, uh, the engineers are all very happy about the idea, but, uh, the sales department actually does a first because, uh, they, they fear that, uh, customers will actually, uh, actually also use that to, to start debating, uh, service level agreements and things like that.  
Felix    00:10:35    But that's where we actually also want to want to spark a certain mind shift. And, um, so with the open state health monitor, we actually, um, work with our CCPs together to, to make ours more, more visible and transparent and use that as a way to, to build up trust among each other and also stop seeing each other as, as competitors. And, um, basically the idea behind the <inaudible> Health Monitor is that no measure what you manage and also be transparent about it. And, um, it's basically behavior. I call it behavior based monitoring. So the eyes of the customer, because basically we don't use any hidden APIs, we just do what each and every customer could do also. And, um, we, we started, uh, collaboration with the fellows from the open telecom call. Cause uh, that's where the open state Health monitor originated, uh, five years ago.  
Felix    00:11:30    And, uh, they actually developed it further. And, um, it's now another project stackman on GitHub where we work together. And, um, that's, um, that's one of the, one of the aspects that we actually want to do is, um, spark, um, sparks the idea that we, we work together on also on these things. But, um, I'm right now very much talking about tools and, um, the, the question that we really wanna, wanna raise is, is it enough for, for something like, uh, open operations to just use or just publish runbooks playbooks, uh, source code, uh, because that's basically still open source development and, um, what, what we actually thought, or what we think is that, uh, that, uh, the crucial part is sharing and documenting best practices for operating cloud Stack. And, um, that's actually, um, where, where we really want, wanna tackle the, the problem that we see.  
Felix    00:12:36    And, um, I tried to explain that to, to someone else a while ago. And, um, I drew a pyramid, which is basically, um, on the bottom people next layer processes and on the top tools. And, um, and when, when we discussed it, I basically, I applied what I call the, the iceberg effect. And it's basically that, um, it's very easy to, to talk about tools because, um, talking about tools and sharing tools is usually not very controversial. So, um, of course in, in larger corporations, you need a process to somehow open source your scripts, legal has to look at it and, and all these kinda things. Um, but that's fairly trivial compared to actually opensourcing or opening your processes. So, um, basically opening the, the processes and making those more transparent. It's, uh, much more controversial than, uh, just throwing the tools over the sand over the fence and publishing them on, on GitHub.  
Felix    00:13:43    And, um, for small companies it's usually easier, but the larger the company gets it, the harder it's actually to, to open up about processes and, uh, live them also in the public because for, for some reason, people are afraid of being, if they, if they live this kind of stuff in the open to open up more tech surface. Um, partially I would say that there's also something that, that needs the mind shift in, uh, in the overall culture, um, because basically customers should not abuse this kind of openness. Um, but, um, so the, the more you, you go down in the pyramid, the, the more controversial it gets. And, um, if you actually talk about, um, the, the people, um, there is, um, the, the big term of psychological safety, um, that in a lot of, and I think actually in, in a lot of IT companies, the, there is already a shift towards, uh, what I would say is the a healthy our culture, um, so that people are actually not afraid of, um, of raising mistakes right in the beginning instead of trying to, to hide them and, uh, actually sweep them under the carpet.  
Felix    00:15:05    And, um, there's, uh, a book by, um, Amy c Edmondson, um, from Harvard Business School. It's called the Fearless Organization, that actually dives into this whole subject of, uh, how important it is to, to establish, um, psychological safety and how she backs that up with, uh, certain studies, um, that she did, for example, in a hospital where basically the teams that, um, that reported more mistakes actually worked more efficiently. And, um, there are tons, tons of examples for this. Um, and, um, from, from me personally, if, if I'm in a place where I'm fairly new, I'm usually at the beginning very shy to actually point out stuff that I, well, I have a gut feeling, hmm, this doesn't sound right, but I'm usually a bit shy of actually raising it and, um, turns usually out, um, later that, uh, my gut feeling was right and I should have just, just raised in the beginning.  
Felix    00:16:07    So that's really important that, um, that there's an environment where, where people are actually, um, enabled to raise things very early and have no, no fear of speaking up or being marked for speaking up. Um, there's also one big case study about that is, uh, what happened in the development of the, uh, several Boeing planes. Um, well, that's also because of lots of pressure. People make more and more mistakes, but nobody was, uh, was basically allowed to talk about them because then they would've had to go back and fix stuff. And, uh, that would've meant, uh, lots of money lost. Um, and, um, so, um, one item I already mentioned is the whole site reliability engineering movement, which, uh, basically in a lot of ways goes into the, the right direction, um, already sharing this kind of stuff. And, um, what, what we now started at, uh, the Sovereign Cloud Tech project is, uh, the open operations manifest@openoperations.org.  
Felix    00:17:13    It's still, um, we are still in the final phase of drafting, um, but um, we are now actually starting to, to go out outward and actually talk to other people about this and see that people adopted and, uh, actually carry on the message and also start talking about that. And, um, one, one aspect of the, of the open operations manifesto is, is we build a community of, of practice. And, um, what, what we actually have in the, uh, Sovereign cloud tech project is that we have, uh, every four weeks we have the, uh, lean SCS operator coffee, which is a format where, where ops people from various CSPs are running the reference implementation come together and actually talk about, um, how they run it and how they run into problems. And, um, they actually exchanged all their hurdles. And in the last release cycle, what we actually saw is that, um, two of the CSPs actually sat down together to update, update each other's deaf environment together in order to learn from it.  
Felix    00:18:24    And, um, that in an environment where usually people see each other as competitors is, uh, is really awesome. So, um, and it actually enabled us to make a much better release because they, they found quite a few things that we then fixed for the release and also gave us the feedback that the overall stuff was really working well. And, um, that's what, what I, our community summit, um, I labeled as a collaboration over competition because, um, we wanna make sure that people understand, or that also the c piece that are active, understand that the, the cake that's available at the buffet is large enough for everyone. So it's not like that we actually steal each other customers. Of course, there are customers and there always will be customers that move from one CP to the other, but compared to the overall market, that's such a small amount that we shouldn't worry about there.  
Felix    00:19:19    Instead, we should really focus on building these community of practices, sharing our whole Stack of tools, processes, how we build up people, um, to basically overall become better. And, um, so one, one aspect is to rebuild the community of practice. Um, we share knowledge, um, that we actually share all the stuff that is built. And, um, there's, um, there's a quote from Tim Riley, the founder of the, uh, O'Reilly Publisher Publishing House. And, um, at a conference, um, it was a <INAUDIBLE> in 2004. He back then said, said, create more value than you capture. And that is something that we, we wanna spark in, in the community to work with it. Um, each and every one of us actually goes out of their way to create more value than one sell captures. And, um, so I already mentioned, uh, the Lean SCS operator coffee. Um, we had the, we have various pairing sessions where, where we work together with, with the CSPs or where the CSPs work together.  
Felix    00:20:27    Um, then, um, the, um, we have several special interest groups that, that we established. Um, some people are also know that from the open context where they're also special interest groups such as the large or the, um, public cloud. Um, we, for example, have a special interest group monitoring where, where the operators come together and discuss the needs for observability and, and monitoring. And we then make sure that we actually do the proper development upstream, for example, in caller Ansible or similar, and make sure that it's actually available to everyone, not just, um, people that use, uh, parts of the SGS Stack, but also basically the overall open community. And, uh, right now we actually start with, um, talking about audit logging because, uh, all the CSPs have the, have the same need to, to know where information is actually popping out of the Stack to either make sure they, they are aware of it for GDPR compliance so that they actually can put a proper retention to it, or that they actually know what's available in case of debugging.  
Felix    00:21:38    And, um, then, um, of course, um, one quote, um, that's actually from Art Kovski, um, one of the former open BD developers is that, um, we believe thats make us experts and it's has tons of titles. So some say fail fast, fail early. I actually like, like we believe that failures make us experts because only through actually making mistakes, um, one becomes overall better. And, um, that's something that, uh, the companies where I, I worked and work, I, I usually try to teach, um, teach them. And again, it only works if, um, if psychological safety is in place. And, um, one, one buzzword is blame blameless postmortems, um, that's out in the industry. Um, there are actually two really good, um, root cost analysis available that we like to quote in that part. And, um, I've, I've already talked to people that are also, and I, I know from the past places where, where publishing a root cost analysis was, um, always a bit of, well, then, then the customers know that we screwed up here, would've made a mistake there.  
Felix    00:22:58    Yes. But, um, if the customer knows that you did that mistake once, if you learn from it, the customer can also be sure that you won't do that mistake again. And being transparent about it is actually what, uh, what enables trust from the customers side. Um, I said earlier that opening processes is something that companies are usually see a more bigger difficulty in. There's one really good example, uh, GitLab GitLab actually has a handbook out and, um, uh, we are working now with one of the companies within the STS context that also wants publish all their, their processes so that others can actually adopt it. And, um, in, in Germany we have, uh, certain certifications that you can run through as a cloud service provider. For example, the, uh, ISO 27 1 or seven eight, as well as the, uh, B bs I C five, which is, um, one of certification certifications that only few have.  
Felix    00:24:00    And by basically also, um, publishing more on that, others are unable to, to run through the same certification. I actually learn from it as well. So that's also good. Um, and the status pages I added there, um, it actually, we, we, um, there are tons of status page project out there and we actually identified that, uh, none of them really suits, um, all the CSP that we talk to. And so we actually right now in the process of making sure that there's, uh, also a status page, um, application available that fulfills all the needs that our CSPs identified. So we're actually sponsoring that development right now. And, um, yeah, so open operations.org is where we publish the, the manifest in other resources around the, uh, open operations initiative. And, um, SES community is where, where the Sovereign Cloud project is found, and we develop all the stuff that we do on, on GitHub. So that's there. Hello. Two minutes to spare time for your questions, I guess. Well, and, uh, I guess there should be, oh, there to chat here. Um, and actually, um, that slide should feature also my email address. So basically if you, if you're shy now or wanna reach out later, feel free to drop in email to fk alliance.com. Um, or you just type in Google Felix chron and he'll find lots of ways to get in touch with me.  
Felix    00:25:57    Um, if there are no questions, um, I usually refrain nowadays from introducing me in the beginning with a long about me slide because I don't wanna bore people. Um, if, however, I, I'd usually like to know who's actually talking, if I'm sitting in the audience, um, to also know a bit, uh, on, on the background. So, um, I'm, uh, I'm born in year 80 and I started, uh, doing this kind of stuff when I was in 12th grade and founded this I p and it's, uh, that was 98. And since then I've basically done a lot of open source stuff. Um, been, uh, open BSD developer for quite a few years, developed some appliances, is based on open bsd, um, worked in the open Darbin project with some of the, uh, apple people. And um, also was one of the people that ran a larger CSP over the last four years, um, as the technical side, as the technical managing director. And started working with the Sovereign Cloud Tech project, uh, February this year. And I'm there, I'm the PO for the infrastructure of the service layer and, um, but I'm also a member of the extended board of the Open Source Business Alliance and has been for the last, uh, six and a half years. So, um, that's actually one of the things that I, I do also in my spare time. Yes. So any questions  
Felix    00:27:23    Or was I, was, is that boring that, uh, everyone fell asleep?  
Thorsten    00:27:30    No, I think you were just so deep into the topic that the no questions were left open.  
Felix    00:27:35    <laugh> <laugh>.  
Thorsten    00:27:38    Okay then, um, yes, I put all of the links in the chat. They will be all available in the YouTube video a little later this week. I appreciate all you coming here and I am ask you please two, if you want to subscribe to any of our different channels we have, this would be amazing. Second, I would really laugh if you would, um, have a look at the first, um, um, 2023, um, deaf room about the so Sovereign cloud and, um, data privacy and things like this. Maybe you're interested in having a speak or a talk there, or a lightning talk, something short and  
Felix    00:28:28    Or virtual feather session. We can also have virtual of feather sessions, so, um, that's also a very good place to discuss things and, uh, throw up ideas and debate,  
Thorsten    00:28:41    Right? Like, great. And last but not least, if you want to participate in any way, um, then here's the guitar of Operate First. You have select channel. You can suggest a topic here. And I would also be happy if you can take the survey about this meeting here and bring us new ideas that you're interested in. Felix thank you for your time and, um, looking forward to work with you in hopefully two future sum ups, uh, summits. I'm sorry, <laugh> and everybody else. Have a wonderful rest of the Tuesday. Bye-bye.  
Felix    00:29:20    Bye. 
