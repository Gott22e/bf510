---
title: Algorithmic Bias
---

# Algorithmic Bias

**Adam Labadorf (00:00:37.980):**  one more minute. Okay let's get going. Alright, so today we're going to be talking
about algorithmic bias, how many of you have heard that term before a couple of things yeah. And there's no math in this
lecture, just in case anyone was worried and i'm sorry if you're disappointed if there's no math in this lecture, but
this is kind of a conceptual discussion are called covering of many of these this very complicated. issue but dedication
today's to Joy will and weenie she is a Ghana American your scientist and digital activist, I think she's still at the
MIT media lab across the river and she founded this algorithmic justice League, which is. it's an organization that
identifies and challenges bias in our information systems, she has this great Ted talk and i'm going to i've learned
this from Fred I kind of like playing videos so we're going to play a minute of her giving her Ted talk.

<iframe width="560" height="315" src="https://www.youtube.com/embed/UG_X_7g63rY" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture" allowfullscreen></iframe>

Joy was motivated to approach this problem when she noticed that some facial recognition software and didn't work on her
face but did on her white colleagues. 

Data is now required for many aspects of our lives. They are involved in our civic life, demographics, geographic
distribution, schools, political affiliations, our economic status, our income, the products we consumption, our credit
scores, our loan rates, purchasing habits, social networks, social media. The information that we consume. Our
Internet usage is being tracked all the time and sometimes it's useful and sometimes it's scary. And then of course the
probably some of the most influential data is about our medical and health. Our insurance claims, how to diseases travel
in certain places, who has access to health care, what is our life expectancy, our birth rates, how much pollution are
we exposed to and how does that influence health. All of this is increasingly encoded as data that is collected and
generally used for not overtly nefarious purposes.

But one of the biggest problems here is that the systems that collect this data are proprietary. This means that you
could ask Google "give me all the information you have on me" and they wouldn't give it to you #unsubstantiated. Same
thing with Amazon, same thing with hospitals. So, even though data is central to our lives we don't actually have access
to or control over the data on us.

In general terms, anytime you have data and want to do something useful with it, you need to have an algorithm.
Algorithms are not "bad" but what exactly are they good for? Broadly speaking, algorithms help us in a number of ways:

* **To scale decision-making.** People and organizations need to make lots of different decisions all the time,
  often there are too many decisions to make by the number of people available to make them.
* **To eliminate the need for humans to make certain decisions.** 
* **To make better informed decisions.**
* **To eliminate the influence of human bias and fallibility (in principle!).**
* **Discover new solutions to existing problems that human ingenuity couldn't yet solve.**

There are many ways in which algorithms are beneficial to us. However, it is how we use them that is the most important
thing.

So what do we use these algorithms for just in a general sense? Of course there's Google search results, Amazon product
targeting, all those sorts of expected things. But algorithms are also used to determine whether you get a mortgage and
if you do get one, what is your rate. Algorithms are used to match medical residents so with hospitals around the
country. They decide who receives limited social service resources. They are determined college admissions. They guide
judges on prison sentences based on risk of recidivism. And they even determine whether someone qualifies or not for
insurance reimbursement. There are algorithms underlying many of the decisions that affect our lives so clearly these
algorithms have a tremendous amount of power. We use them in various ways so let's step back and talk about what an
algorithm is at its core.

For the purpose of this course, we define an algorithm as a precise sequence of steps that transforms an input into an
output. Basically, this is the proverbial black box: you put data into in, it does something to it, and it produces some
output.

![Basic algorithm definition](algorithm_definition.png)

The algorithm should work in the same way regardless of what data is provided as input. So the idea, then, is
that we like to think that algorithms are so-called "objective" for this reason, in the same way that we like to think
of science as "objective".

Algorithms in particular have these very attractive properties in that they're discrete: you have to tell the computer
how to do it, so does this thing first those next. Their explicit, like you, writing code will talk about sometimes you're not we'
ll talk about that later, but each step is explicitly defined and therefore, in principle, understandable. And
repeatable So if you just push the button, you should wear the same input, you should get roughly the same output. And
these I think these principles are actually rather attractive, but they do, in principle, allow us to avoid subjective
mistakes say or human intuition from our human judgments. So what is not
written the bus will algorithmic borrowing from Wikipedia here i'll rhythmic bias describes systematic and repeatable
errors and the computer system. That create unfair outcomes, such as privileging one arbitrary group of users over
others right, and so the key words in here are systematic repeatable errors and unfair and arbitrary I guess those
things. And so, how does let's talk about an example of an algorithm that is used to. or a number of algorithms that
have actually been shown to encode bias, I mean have you heard of this pompous or. This this Was this a pro publica
report came out about this pompous system, the pompous system correctional offender management profiling for alternative
sanctions is it's a computer program that judges us to decide how long sentences should be for people that they are
sentencing. And it's been around for a while, in 2016 this journalistic organization pro publica did an investigation on
the software and they discovered that it was systematically bias against black people assigned them longer sentences
for, then there are equivalent white offenders. There are instances of inequity in medical treatments, so one of the
diseases, I study is chronic traumatic encephalopathy it's the nfl head injury disease. And it is like somewhat
shocking, the rate at which nfl players have experienced this this terrible disease later in life. and The nfl was very
reluctant very reluctantly was made aware of this, and this was made adjustments, and so they did. come up with some
sort of a payout to people because based on how much CTE they got as a result of playing and there were these claims
that retired black players say that their payouts were less than like letters. black people have trouble trying to
refinance loans and in this in this story, I mean I i'll say I just kind of like. I didn't look very far to find these
stories right you just type into type it into Google and these things come up, so this was in the story, there was a
black man who had you know great credit. Great stable work high salary everything and he was disallowed from refines
anything from refinancing his mortgage because the program called the loan officer that he did didn't match the third
criteria for refinancing. And even when we are aware of these biases and our systems and we tell our systems, not to be
biased. The bias persists, so this is an example from so facebook's algorithm discriminates even when it's told not to
say fine, so the story behind this. Is Facebook has this algorithm that targets ads to people and they license this
algorithm it's semi proprietary like it has a special sauce. That they don't tell everyone about it, but they tell like
marketers people were trying to sell stuff basically how it works. and companies can tailor like they can decide they
can they can tweet settings and this algorithm to say, I want to target this group of people, because they think those
that group is more likely to buy their products. Well, they used to have, I think it was like ethnic capacity as one of
the settings in the Ad Program. and eventually the I think the US Government sent them a cease and desist on that
variable so they remove that variable from the algorithm. But they were still the ads still targeted like certain types
of ads to certain groups just removing that variable from as a selection was not enough. To eliminate the sort of
biases, and these were you know somewhat permanent pernicious things not necessarily intentional as we'll talk about,
but then things like targeting high interest rate payday loans to people of color there is a much higher incidence of
that sort of targeting. And just more risky types of and and certainly less certain some less scrupulous businesses end
up getting targeted to people of color. So this is it's a really. sticky problem and we'll talk about some other reasons
why so first so far i've been talking i'm going to talk a little bit more about types of algorithms. For the purposes of
this lecture i'm going to say there's two broad classes of algorithms there's human driven. So we're there's programming
bias, how many of you have written code to you any of you don't know what your background is a little bit. So don't
worry about it but programmers what we're doing is we're taking some sort of model of the world and we're putting it in
writing it rang expressions that you can understand that represent our belief of the world. And those beliefs, are not
always obvious to us right, but many of them are implicit. But, in general, since a human wrote it in principle, another
human can read it and understand what it does right, and so this is like the traditional algorithm design. Recently, and
i'm calling this human driven but recently machine learning Ai deep learning, you are have all heard these terms. has
introduced a whole new class of algorithms and the idea here is that the algorithms that are used on data. Are not
specific to the data a human hasn't gone in and said, I want to like if a person has these the US a human is not setting
the rules of the code these algorithms are generic you give them a bunch of data, you say this. Is representative data
build me a model that encodes the patterns and that data. Right, so the algorithm is designed to accept many examples.
The data is summarized in some way by the algorithm which is again generic. And then the idea is once you build this
model with existing data and you get a new data and you ask what okay algorithm, what do you think of these data. And
the difference with this is that these models being generic can be very difficult or impossible to understand how many
of you have heard of deep learning. How many of you have ever done any of it. A little bit It is crazy complicated like
it's the deep learning. These algorithms are patterned after the way we thought neurons work. Basically, have the same
sort of an analogy of nodes and connections between nodes and information flowing and activation of these different
nodes and there's all sorts of different types of layers and like it's really, really complicated. And the more
complicated the model gets the harder it is for even the people who build the models to explain how they work they're
just like I don't know we all know what this means, but it gives accurate results. This is the so called explain ability
problem we'll talk about this a little later, but. These data driven models that we're using now ubiquitously or can be
very difficult to explain and this is what we call artificial intelligence and machine learning. So, from now on we're
really going to be talking about both of these, but just know that there's a distinction. So some basics about machine
learning so machine learning is a subset of artificial intelligence. machine learning is sometimes called statistical
learning because that's what it's doing is taking numbers and it's expressing them and encoding them. And summarizing
them in such a way that you're sort of learning up an internal legal representation of the statistics of the other
numbers. And there's an error, the algorithms themselves don't know for me to know anything about the meaning of the day
right like you'll build a deep learning algorithm they'll train it on. health data or we'll train it on economic data or
stock data, but the algorithm itself doesn't care what type of data that is. These algorithms learn the sort of linking
structure and the data you're saying here's a whole bunch of examples shop give me something that expresses the
patterns. And so, therefore, and this is key, each one of these models is specific to the data that there was used for
training. And so, therefore, and machine learning algorithm can create an infinite number of months, like there's an
infinite different. data sets out there and so there's an infinite number of models there's nothing necessarily right or
wrong about a model there's an infinite number of them. And then some models, depending on how they work, some
algorithms will create different models, with the same data, there might be some random component to the algorithm. And
so, whenever you like. Right so let's go into just a simple illustration of this right. So let's say you are interested
in, you have an image classification problem and you want to have given an image you want the computer to tell you, if
it's a peanut butter and jelly sandwich or not, so you go out you find a whole bunch of examples of peanut butter
sandwiches. And that's great, but the algorithm also needs to know what is not the peanut butter and jelly sandwich so
you have to give it examples that are not peanut butter sandwiches. So you do that, like finding things that are almost
certainly not peanut butter and jelly sandwiches you say, these are the non representative biases, these are the
representative classes find the features that are specific. And some of them might be similar like a regular sandwich
might be fooled right, but you never know. And this is that what you're trying to discriminate the out you're asking the
algorithm to find what makes these different. So you take all this data, you put into a black box. And now you have a
new picture of a peanut butter jelly sandwich or something you put it into the black box and you ask it is this a peanut
butter and jelly sandwich or not. This is fundamentally how all of our machine learning algorithms work you give it a
whole bunch of data we've asked you to learn the patterns of those data and then you give it new data. and have it help
predict what you should do help guide your decisions, so this is the the whole background behind algorithms as i'm
reading and so there's another style of. machine learning algorithms. That goes one step further. How many of you have
seen defects. it's all explained, with the fakers. photo or video of something that never existed right, so another one
recently with like zelinski saying how really not you know are. backing down from this one of the big never said that he
never recorded that video but it takes, you know, a bunch of photos right have somebody say will be in one day, and
maybe like obviously always new stuff and then you put all that in entitled to spit out. Right, and so this is exactly
deep fakes our so called generative machine learning algorithms generative because the model itself can generate new
examples. And so that's the second style and so instead of giving it, you know directly just a picture of what it knows
about. The black box has learned some kind of representation of what a peanut butter and jelly sandwiches So in
principle the black box could be used to construct new peanut butter and jelly sandwiches. And that's exactly what the
fixes you train it on I mean it's it's more complicated than that. But the idea is that you use this black box and you
say here's the pieces like audio and images and then make me something that fits what I want. The technology that
underlies this process is actually be how many of you have heard of does anyone know the type of specific technology
people use for this. it's called adversarial neural networks. it's actually really creepy so the way adversarial models
adversarial neural networks, work is they're actually two. Models there's two algorithms the first one produces an image
or text or something and it tries, and then the second one tries to like it tries to fool the second one into predicting
that its natural. True input. So this first adversary produces some output, it tries to convince the second
classification, that is right, and then the second classification algorithms like well at the beginning of person
talking to be right and there's no that's wrong and it tells the first one, no that was wrong. And the first one can
refine this model and it tries again. And it keeps doing that, until it consistently fools the second one. that's why
it's called adversarial it's it just does this over and over refines the mall, to the point where the second adversarial
neural network can't isn't fool anymore, which. creepily often works on humans to. you're not looking really closely at
a defect like. You could easily be full will happen. So that's how that's how this works, and so this is, I find this
particularly scary this technology like it's sure it can be really useful for things but. what's, the first thing it was
used for but like trolling people and doing awful things course. I don't know what I mean, I guess, but in principle,
any problem that you would want to try to solve like this, you could use this adversarial in there on that doesn't have
to be in affairs. But of course that's the one I mean all. Right so so far, what is the summarize. In both cases, so I
remember, I had a human driven algorithms and data driven algorithms at the end of the day, computers only do we tell
them. We either tell them what the sequence of steps should take the data and transform it into an output, or you
specify the data, the model should learn give us the output. And, of course, what we tell our computers to do is not
always what we want them to do, and this is where the law of unintended consequences, so this is lesson number one.
Alright, so this is sort of a simplistic graphical representation of what an algorithm is many of you may have heard of
garbage in garbage out. Of you how many of you heard that term know it's mostly in computer science, do you have a
program that's perfect does everything right but you're giving garbage the APP that's going to be garbage. And the same
applies for advice, but the data you put into an algorithm is biased, then the output, you get off is going to be biased
unless you're careful about it and that's what we're going to be talking about. So earlier, I sort of mentioned these.
sort of appealing objective properties of algorithms, but of course they're not objective, because we specify them and
the way that I mentioned, either we write down the list of steps, or we pick the data, where we do both right. And these
algorithms have no knowledge of the world except what we tell them or what we encode in them, and the results are
interpreted and put into practice by us. there's this this notion that like in this pompous thing like this compass
algorithm that helps judges decide how long someone should be in prison. The Duchess doesn't have to respect that. Right
like they could say no that's too long. they're not legally bound to use the opposite of algorithm, but they do. Because
I think they say, well, well it's an algorithm the algorithm told me to do it it's obviously you know better than I am
so it knows more than I did, and it has data in it so but that's you know it's still a choice, but we can still our
human judgment can intervene in this. But we often forget that it seems. And so the last probably most challenging
aspect of algorithms and this. scenario that I described is is that they're highly susceptible to feedback loops we
talked about this last discussion, but i'm going to go into a little more detail about those. So this is a figure that I
invented to try to illustrate what I mean about feedback loops. Right, so we have this world, and this world right now
is filled with data it's generating data all the time there's lots of its pre existing data in it and so these
observations, go into our mental model like what do we can see as the world how do we think it works. And, and we take
that model of how we think it works and we we decide to specify an algorithm either by choosing the data or by writing
the steps. And the output of those algorithms because we choose to use it inputs data back into the world. So I call
this the so called model right we're interpreting the data from a particular lens, namely our. conception of the world,
we were coding some aspect of that conception into our algorithms which then controls and determines what happens in the
world, which then looper feeds. there's a second. And because, of course, you know the data that's produced is
consistent with our model may or may not be consistent with our mental model, and so it reinforces that that. that's the
model, the data we is all about the data right, because when we make a decision based on an algorithm and it puts more
data into the world which is collected and then that data gets fed back into our algorithms. And so it's actually when
you think about it this way it's pretty obvious that the is the systems can can persist and this isn't necessarily bad
we'll talk about that later, but. The question is, how do we circumvent these feedback loops and there are ways that we
can, if we're aware of the biases in the world itself, we can adjust our algorithms to remove bias, or to D bias or data
will talk about this in the next section, so this is one place where we can intervene. Right, where we see these
observations, but we know like black Americans have higher in person ratio incarceration rates. If you just look at that
and you might think that black people are more likely to commit crimes, but if you know more about the system, you know
that the system has been. Designed basically to for that to be true, and so you can interpret those observations
differently if you have that knowledge. The second place, that you can intervene in this loop is when we specify our
models, so we have our conception of a model and now we're telling a computer for encoding that model into. Well, we
have full control over what that algorithm does, we can explicitly incorporate aspects of. equity into our algorithms
themselves, such that the outputs are less likely to be biased to reflect historic biases or on desired biases so we can
indeed. In principle. Intervening in these loops. But of course the, the devil is in the details so lesson number two.
algorithms used to make predictions about the future use data from the past that doesn't sound too controversial, but
what else what other data would use, but, of course, if you do that, that means the future is going to look like the
past, and this is. It sounds obvious when you say it, but I think we often forget that right like we are when we make
right algorithms to make predictions and then use those religions to make decisions we're saying we want the future to
look like the past for not conscious about. And so you wonder why. These issues persist so that's the background I think
that's that sets the stage for this next section going pretty fast to this. Question so far, this is all very abstract.
So the question is. What we do about this. I know, none of us in well, I guess, I call myself a data scientist, so I
mean that's what those are my these are my tools. But not everyone has those tools or is going to be doing that so. What
sort of the, what are the ideas and strategies and challenges that we, as citizens can try to keep in mind and embrace.
So this this was originally two lectures and so i'm going to pause and do the dedication again so timmy gebru she is an
Ethiopian American computer scientist. She she lived in Massachusetts when when she first came to this country from
Ethiopia. And she made her way to apple thing or Amazon or Microsoft I can't remember which one and then she moved to
Google, she was recruited to. into a group that was concerned with ethics. At Google. He wrote a paper that was critical
of a new language model that Google had built and under somewhat mysterious circumstances, she was ousted from Google.
and She, and so I don't and I think this is in the past couple years, so this is pretty recent. haven't you heard of her
or Great we're trying to unsung heroes. And she was the founder of black in Ai so she also did this got into this field
kind of rapidly like she was going to all these Ai conferences and she noticed that there were all the black people and
so she. gathered them together and founded this black and Ai group that is meant to be a an inclusive and welcoming
environment for for people of color and just because Ai computer science, in particular, is really, really biased
towards female being a man and being white. Biology is not so bad, as I understand it, but these fields are very, very
heavily white now and so definitely something with me. i'm not sure what she's doing now. Okay, so after the first part,
so we talked about algorithmic algorithmic bias analysis. How do we mitigate this and in sort of a conceptual way right.
Just as a reminder, I mean I don't really need this very talked about this, but again, this is two lectures last time.
So we have this notion of an algorithm just accepting an input in producing an output, we have input output garbage in
garbage out and also by us and by us out, which is also garbage. And we have this loop that we just described. So. Where
did I do this right there are all sorts of sources of bias that can cause these problems happen. And there because the
world is biased and we collect data about the world the data biased, so we have all these historic biases, which is
exactly what this course is about. But there's other types of buyers as well, so general sampling bias unit, but you
guys sort of sampling bias, basically, like the sample that you have collected is not representative of the larger.
population. And even if it is representative, if you don't sample enough of it to get up the pattern then you're going
to be misled. And sampling so sampling error as well you know, resulting in incomplete or imbalanced representation, so
it might be that some of your classes that you're trying to sample are actually just relatively. less frequent than
others, so I think in this country African Americans make 18% of the population 1718. Something like that well they're
just going to have your data points in an equally sample this out because there's fewer of them that's not necessarily a
bad thing, but then there's less data on those groups. And there's some information that is just really difficult to
capture i'd be if this came up last time I think Abdul brought it up it's like what are all these measures of. Like. All
the different measures that they were using to calculate. disparities. Like you can capture some of those things we
patricide you have to assign numbers to them in order for these algorithms or so, how do you do that, but it may be the
case that the information that you need isn't actually collected, how you know that. not easy. So these are databases,
but there's also model biases and again historic human biases Dr into this, what is our conception of the world, how do
we think the world works and then, how do we therefore behave in the world. The model produces the results, the tree the
arbitrary groups unfairly right, this is algorithmic bias, but it's generally just a human bias right like that's kind
of what this class is about as well. The models that we build may not be trained with enough data they not be not be
trained with representative data and models may not be equity aware right, so this these things there's all there's all
sorts of sources of bias throughout this whole process. And so, how do we mitigate this well there's kind of two ways we
can think about this, we can either be proactive and be aware of all these ethical biases. and try to design our
algorithms responsibly there's a book called the ethical algorithm, which is a little technical, but it is a about these
techniques, if you are tech company. And you somehow feel obliged to make your data and your algorithms more equitable
What do you do, how do you do that. And so you can actually be proactive in this process. Particularly when designing
and conducting conducting studies right collecting your data, how do you collect data in an equitable fashion. But of
course you can't sample everyone every every company every situation study has limitations, so you have to pick a
representational subset This is where some sample bias may come in. And if you're lucky, you may have the demographics
of your population, so you can include that in the process, are we, including enough of the different groups that we
wish to include to have enough statistical power to compute reasonable summaries. So you can figure out what the
distribution is what how old, are they what is he what is he drained what is education range well the things that you
think are important and then you try to subset. As many people, as you can sample as best you can. But of course we're
constrained studies are expensive. And you may not always have all that information about the people you're trying to
sample. Like how many of you have been on a TEE and there's a an ad that says here volunteer for this study. Like are
they targeting people who write a deed, which is a lot of people. But they that clearly they just don't have enough
resources to to enlist all of the machinery needed to identify people and reach out to them and, like and go through
that process so. Many of these studies, you get what you get and so being proactive is not always possible, in fact, and
Problem Solving possible through proactive in the data that we're collecting. And even if you do have control over some
of that so. As opposed to proactive the mitigation more often, we have to be reactive to mitigate these biases so the
data already exists, and often the data are collected by other people, so we didn't even have an opportunity to have
adjusted or controlled those data samples. And so, that means that we have to be extra intentional about what does the
data contain what does it mean. And how can we use it responsibly. So, and also one of the populations that the data
represent and does that fit the data that the population that we wish to target like there, this is this happens all the
time in biology we're not even talking about people here like someone does some sort of. experiment in I don't know
breast cancer in the population of people for some particular purpose. You may also studied breast cancer, but you may
have a different purpose. it's really important to understand what the conditions were in that initial experiment to
know if those data can be posed, for your. Typical experiment and it's not really straightforward it's not always clear
but that's true, but you think i'll dedicate the breast cancer data set, we can use that right, are we not, or maybe
not. But here we're talking more about demographics right so data collected from people. So what are the key variables
that we have to consider how do we do we have race do we consider it is that important What about socio economically
from what about education level health health impacts, do we have those variables and can we consider them. But have you
have we mentioned proxy variables in this class. know. A lot of techniques lines. So a proxy variable so remember that
the example of the Facebook algorithm targeting issue right ethnicity used to be a drop down. And then they removed it,
but these issues, whose these biases remained. Well, there are variables or proxies variables for ethnicity and race,
where you live, your zip code depending on where you live, is a very highly predictive of race. or socio economic status
you're. All these different things that we were talking about in the discussion is you don't need to include race you
don't even need to collect it. Many of those things are already encoded in the data and the other variables, simply
because of those associations, those are proxy variables. And they can be really tricky like, how can you tell if
something's a proxy variable you haven't measured risks and. So these are things you have to keep in mind whenever
you're looking at this like Am I using race card intentionally through these other variables that may be in the data.
And you also have to cook yeah so all these things you know you have to either distributions of the variables of
interest they match what you're interested in. And then, this is a very instrument type question you know what groups of
people might be helped or harmed by the results and there's a huge like very deep ethical questions problems that you
encounter people down that rabbit hole which we're not going to do here, but. And then you know, finally, these are
where the data collected in a way that introduces system advice for our purpose right, it may not convince the stomach
for their purposes, when it was collected, but it might be for ours. So these are just questions, all these are
questions I don't I think we are still we're at the forefront of like, how do we actually do this I don't there are far
more questions in our answers. So one of the ways and so all right, so this is reactive, most of the time you have this
sort of reactive on situation, but in both proactive and reactive, one of the key concepts about a data set in
mitigating bias is by protecting certain attitudes. Protected attribute is a variable that partitions people into
groups. And that each one of those groups should have some notion of accuracy equal treatment right let's say you divide
people into people of color in my people. If the output of your algorithm. doesn't treat those separate groups of people
similarly then your algorithm may be biased in that case, race, would be a so called protected that protected attribute
are protected variable, but it can be many things like gender, sex, religion, past depending on where you are. These
protected attributes are things that we need to be aware of, and this is not technical right, this is conceptual this is
ethical, we need to identify variables that we want to make sure. treat people fairly. And so just in terminology here a
group is a set of data points examples, or you know people in a data set of corresponds to the same protected attribute
values right all black people all the spam people all one people that's a group. And the privileged value of a protected
attribute corresponds to a group that has historically then systemically advantage privileged value right, so in this
case, it was racing would be white people that's the privilege battle. Alright, so we have this sort of this notion that
protective variables and he's DSS that may be in balance, they may have sampling bias, and so, how do we know this
original. The first way that I talked about. Intervening in this process is you can remove bias from your data so. You
can do that by relating So if you have a small room like a low representation of, say, African Americans, you can
increase the weight of those samples such that they have greater influence over. over your results to better balance at
attained Venice sort of notion and. You can change the labels and features so here are features like just on any one of
your. Like any one of the variables that you're considering. You can pre process them, and this is this is yeah in some
ways i'm not going to get into how you decide this is one of the ways, you can do it. You can learn fair representation
right, so a fair representation of data would obscurities protected as. Such that the algorithm can't use it. And then,
finally, is a disparate impact remover. edits the feature values to increase group fairness like you actually edits
values, so this is, this is a current. sounds sounds a little like suspect right, why would you want to edit your data
that sounds scary it sounds like bias. And we'll talk about that. But this, this is just a few of the actual on. A few
of these approaches for unbiased and your data. sounds complicated right. like this is not an easy process and. I read
through some of this literature in the fall and it gets really hard really fast like really deep and dense and
technical. And yet, you know we're all sort of our people in tech companies certainly programmers software engineers
somehow where they're expected to learn how to do these things. Which isn't to say that they shouldn't but it's big it's
a heavy lift to figure out how to do all this stuff, and so the government is actually starting to get involved.
Alright, so this is like unbiased in your data, taking the time to go. I think i'm going to go. i'm actually going to
take a pause here. So let's take a five minute break because the rest of this is all about fairness and how do we think
about fairness. So let's take a five minute break.

**Felicity Crawford (00:49:01.740):**  hey I just heard from listening.

**no speaker (00:49:03.870):** listening.

**Felicity Crawford (00:49:05.850):**  just heard from Melissa no texting her all is well congratulations are in order.

**Adam Labadorf (00:49:13.980):**  You. play felicity you didn't hear from her.

**Felicity Crawford (00:49:17.250):**  I just heard from her right when you said let's take a five minute break.

**Adam Labadorf (00:49:20.910):**  Oh great.

**Felicity Crawford (00:49:22.050):**  There well, she said, your photographs water and Felix things that beautiful.

**Adam Labadorf (00:49:32.160):**  Wonderful.

**no speaker (00:49:33.330):** Day.

**Felicity Crawford (00:50:43.980):**  hey. Adam Melissa says check your email.

**Adam Labadorf (00:51:03.630):**  I just did.

**Felicity Crawford (00:51:04.530):**  Or you did oh good.

**Adam Labadorf (00:51:27.030):**  And during class we.

**Felicity Crawford (00:51:34.440):**  came at the right moment.

**Adam Labadorf (00:52:07.800):**  So he was born this morning at 9am oh.

**Felicity Crawford (00:52:13.230):**  Yes.

**Adam Labadorf (00:52:15.060):**  Not not during class exactly but close enough.

**Felicity Crawford (00:52:19.350):**  Well, we just got to learn about it at the right moment.

**no speaker (00:52:46.140):** one. Oh. Look.

**Adam Labadorf (00:53:22.020):**  At. Whatever they do that was me.

**no speaker (00:53:29.310):** and

**Adam Labadorf (00:53:32.730):**  i'll be.

**no speaker (00:53:37.140):** back. If you're not able.

**Adam Labadorf (00:54:30.000):**  to hang on because when you.

**no speaker (00:54:34.650):** push it on. People. But people not very. incessant. one.

**Adam Labadorf (00:55:03.900):**  Okay let's let's pick back up again. Okay, so so far we've been talking about just
some general strategies. And no real great solutions, but strategies with these or so D biasing our data first right
it's one way that we can adjust our data. But if we do that if we do adjust our data we have the good intentions right
we're going to try to remove to all this stuff we're going to try to re wait for trying to try to optimize reprocessing
are going to do all these things well did it have the desired effect. And for that we need to. Essentially, examine the
output of our algorithm or fairness with respect to those protected variables that we talked about before right, these
are the things we're trying to protect we want people to be treated equally, according to race. But what does fairness
mean. i'll put it to you let's get some definitions anyone want to volunteer definition of fairness. outcome, not just
the quality of your. Life that's how for that, instead of saying okay equity, what does that mean close everything, and
we all push a folly where everybody is saying what even one even even equality but yeah yeah now you say yes. I mean
quality will be regardless of input output. input in Brazilian race or gender ready, but equity would be like yeah okay
so same thing the wage gap right now mowgli love this algorithm is like you know i'm used to populate like a suggested a
range right, instead of just sending out our like. These groups get treated the same like I guess in your design of a
model you're trying to the fact that, like historically input data for women movie lover you know and so it's
compensating. Sure, I mean definitely connecting fairness and equity with the obviously the idea here. Anyone have a but
I mean this is not a criticism, but this a little bit. Vague right there's a lot of details that are specified there. So
anyone can someone try to make a bit more precise definition of we'll get into this I don't know. This is hard. Someone
was to probably the precise definition of fairness. What might be funny. Have a definition on the next slide but wanted
to give you guys an opportunity to think about it. So, clearly the I mean, just like in what you're just saying fairness
equity, they are human values. Right, these are ethical, these are things judgments that we make as human so, how does,
but if we're we're dealing with algorithms we're dealing with numbers. So we have to somehow encode fairness somehow as,
like a number or an expression or something, and so, how do you compute fairness well. there's lots of different ways to
define fairness, both in like a i'm not sure the sentence that. The way you define it was not technical, it was
conceptual right yeah so there's lots of conceptual ways to define fairness. But if we go back to our original like
remember one of the points from the algorithmic bias was error systematic errors. And so group fairness would be equal
error within each group. How often does your algorithm get it wrong that's group fairness. Individual fairness is that
similar individuals are treated similarly, of course, that the devil in the details, there is what a similar me. But
that's another notion right to people who are otherwise equal or are generally you know by some sort of a prevalence
they should be treated in the same way those both seem reasonable. But in any case, you know we're talking about we're
talking about error here and talking about error, and when you talk about area you're actually talking about accuracy
how accurate is your algorithm how often does it get it right, how often does it get it wrong. And we're going to stick
with that definition of accuracy. So accuracy is clearly links to fairness. What did accuracy mean. How often does it
get it right, how often does it get it wrong that seems obvious right but let's dive into that a bit. There are more
than 21 different definitions of fairness statistical definitions of fairness. And as we'll see. Many of them are not
compatible with them. So let's dive into this let's go back to this complex system, so this complex system is again what
judges us to decide how long sentences are. And it has been systematically biased to us to. sentence black fenders. With
longer sentences that was. So the complex algorithm assigns a score to that is proportional to the probability of its
model probability of someone to reoffend. The idea is that if someone is likely to reoffend you want to keep them in
jail for longer so that they have fewer opportunities to reflect that's the idea it uses a pastor arrest records. And
the judge uses the score to assign prison time right. Consider so here on the right there's this model that comes out
like that the X axis is the probability of your offending y axis is the number the density of of the defendants who fall
into that probability, and this was very clearly a bias according to race, so, in other words. there's that there were
more white defendants who had a lower probability, and there were black defendants without lower probability and like no
other way there's more black defendants who had a higher probability and white Defense. So let's be algorithm therefore.
Is know what's what will be one potentially fairway to apply this algorithm well the company believes it's like well, we
should just like assign a probability threshold. Right 30% 18% whatever if you're above that threshold you get your you'
re labeled as high risk of offending and therefore you're given a longer sentence. I mean in some sense that sounds fair
right like you're the same percentage to every person individual saying this. But I mean obviously there's great
imbalances in the the champ that someone will be labeled as high risk of their black and white. And this was actually so
that this was a very public. exchange between pro publica and the company that makes pompous because the company that
makes pompous was arguing that their algorithm Mr. In not precisely because of this, but this sort of intuition right
like there is a sense of fairness that you're saying, giving the same thresholds everybody. But of course it's not. more
complicated than that. So let's see why. It turns out that her definition of fairness depends on what steak you play in
the system. So let's introduce this here how many of you have seen this is called the confusion matrix when have you
seen these. So basically, this is a table that you can create for any algorithm that is doing a prediction right so
let's say you have a bunch of store data of say defendants who were sentenced and then did or did not reinvent. Right,
this is historic. Your algorithm describes a score to each one of those people. And therefore, you have a true response
a true outcome and that predicted outcome. And this table encodes how often your algorithm got it right and wrong in
which way right, so if a person had a low risk score and they did not go on to your friend, those are true negatives,
that means that that the prediction was correct. And if they had a high risk sport and they be offended they had true
positives as of true positives those that the diagonal here is when the algorithm that's right. The opposite diagonals
when the algorithm got it wrong. And so false negatives, means that the person did go on to refund, but the algorithm
did not predict them to do so, and then false positives are the. People who did not reinvent but the algorithm
predictive of the word, and therefore they got one, they will get longer sentences. So this table we're going to dive
into this table. and examine it with respects to a different formula to the variance right, so this is this confusion
matrix true true negatives false positive false negative to positive. So what are the different stakeholders in this
situation right. was involved, someone shot some something out. What people are involved in this. defended. well. who's
making the decision. To judge the judge.

**no speaker (01:06:10.710):** sure.

**Adam Labadorf (01:06:12.210):**  sure. And these are defendants who are suspected of having committed a crime. So who
else is involved. i'd say like I don't know the public. They might care about the outcome. Well let's dive into that so.
or a policymaker to that. So the decision maker, I think, in this case, this is the judge right who's making the
decision. about whether someone's going to stay in in jail for longer. And so, their priority is how many of the high
risk group reoffend right they want to get it right as much as they can. And this is called, so this is the number of
true positives divided by the true positives plus the false positives. So in their perspective, they may prefer to put
someone. gives someone a longer sentence, even if they were not going to reoffend if that means correctly. No assigning
someone with a higher score putting them away people, what about the dependent the defendant. The defendants question as
well as the probability, I will be incorrectly classified as high risk and therefore have a longer prison sentence, even
though there's no way i'm going to read. This is called the this you and calculate this as the false positives divided
by the true negatives positive false positives. This is called, so how often. True negatives false positives is once
again. This is called the false positive rate how often does the algorithm get it wrong when it predicts someone to be a
positive. But you might also be a citizen, so how often are dangerous criminals but back on the street. And this is
called the false negative rate, so you would have the number of false negatives divided by the false negatives into
positives so if we go through this and, but each one of these is a measure of accuracy. I mean they're all you can
reason about how accurate the rp algorithm is but they all answer very different questions. And so what's going to go
through this so true positive that's that if you can think of it in terms of like blocking out rows of your table you're
just saying true positives divided by the some of that home. The defendant you're saying false positives by the by the
summer, with us and then false negatives divided by the summer. they're all measures of accuracy. And this was the
arguments that pompous was made is that, according to the decision makers perspective their algorithm is fair. Because
it balanced out groups within would that optimize that because I mean, who is this offer, for it was for judges like
that's where they're making it far but from the defendants perspective, it was totally unfair. And so, like, how do we
reason about this, these three different ways that i've done this, or more more ways than three to measure accuracy So
then, how do we relate this notion of accuracy to being fair. It means that accuracy, measures must be equal for both
are all groups is protected groups right. So the decision maker from the decision makers perspective, this measure of
fairness is called the predictive parody. If you take the decision makers definition of accuracy and you attain fairness
it's called the compared. To take the definition the defendants definition of accuracy it's called the error rate bounce
affair algorithm will have a fair rebounds and as citizens will be also air rebalance but the other type of air and. So
already we have three different definitions of fairness just from looking at the accuracies of these are just not the
situation. and They all determine so instead of having one, like you, you instead of having one of the major to split
into two or however many groups there are and you're asking of these individual tables are those sensitive accuracy, the
same. Now there is indeed such a thing called group fairness in possibility there. Apparently it's mathematically proven
that if an instrument, so this isn't the case, the test, but decision satisfies predictive parity. That is that positive
predictive value is the same across groups, but the prevalence differs between groups, the instrument cannot achieve
equal false positives and false negative rates it's like Eric medically outbreak we provable. And the prevalence here
means the proportion of individuals who were sedate and given population. Now we do know that African Americans are
certainly arrested at higher rates, does that mean they're committing crimes, no. We don't have that information What we
do know is that there is it it wasn't rate is higher, because they're arrested moral, so this is clearly violated the
two groups whites white people and black people do not have the same prevalence. And so, therefore, you cannot satisfy
all of these notions of badness at once. So the one that gets satisfied yes. And I was making the decision. which was
campuses argument. So what's, the key point here. Is that there's always going to be a trade off between fairness
Madison. You can't have both in all cases. So you have to decide which types of know incorrect was types of inaccuracies
are you're more more willing to accept. mean surprise, surprise, who had the power to make these decisions. Not the
defendant so it's not really yeah it's not really surprising that the situation is whether it is but it's baked into
this fundamental challenge this trade off between fairness accuracy and the various definitions are kind of snappers. If
you find this really interesting, there is a software package out there, that you can use to. implement all these dozens
of different. types of like assessments of fairness it's really complicated i'm not gonna i'm not going to describe this
but, like this is the figure from the paper like this is the system, so if you want to assess how fair your algorithm is
just do that no problem right. But at least there you know you can play with this if you if you so desire. And so we
have all these these points like pre processing that's the the advising of the data, the in processing that's like how
accurate how fair is your model and then post processing is like this is after. This assessing after the fact. My point
is saying is that this is hard. It takes effort and thought. And to me. That. Well we're gonna finish her. Right so.
Clearly equity in fairness our human values that things that we just had they are socially defined their subjective and
their context dependent. And the tools we've talked about so far just tools right none of these tools are answers they'
re just tools and we still need to use our own intuition and our own values to make these decisions with the power that
we have to make them. And algorithmic algorithmic bias simply reflects the biases that exists so it's really. it's not
surprising when it's laid out that way. And, of course, there are lots of stereotypes lots of biases that exist, so this
was another study. Where they were looking at stereotype exaggeration versus mirroring and so mirroring means so
basically does an algorithm output reflect stereotypes. it's not as as chosen output reflect stereotypes and are they
accurate right, so in this study what they did was. The Bureau of Labor statistics is United States Government
organization that collects. Statistics about Labor. and jobs and demographics and they. The data are publicly available,
you can download them look at them, and so what they did is for different professions each marker in the plot is a
different profession. And on the X axis like certain like different professions are important employ different mixes of
men and women. And so the the fraction for goes from zero to one is the percent of women in particular occupation on the
y axis they went on, they had a bunch of people go on to Google. And like do searches image searches for those
occupations and have them just say whether the images that came back for men or women. The idea is that the y axis here
is sort of like a stereotype. Like if you put in I don't know i'm hairdresser. you're probably going to see many more
women pictures oh guess that's my stereotype I don't know, maybe you disagree. But that's that's the idea right and they
had a number of people, I think there were like 20 college students or something they picked them up getting some is to
do, Google searches. And they they collected these data. If the stereotypes in google's algorithm for the same as our
internal stereotypes or reality, I should say, then all these dots would be right on the diagonal. Because the
proportion of men versus women that come back and these different searches would be equal to the proportion that work in
those professions, but clearly that's not the case and some professions are more biased and others. And so, like all
these down here. Present there's a whole bunch of professions that are actually very frequently populated by women, but
no search very few search results come back. With women of those positions, which is not surprising, and there are some
that are the opposite or there are some professions where images of women came back, more often than is actually
reflected. In the workforce. This isn't terrible right like the dots aren't that far off the line. And they're
reasonably consistent, but I mean this is, this is a stereotype bias that's built into google's algorithm right, this is
Google search results so whether or not there are, I mean is there, another search. Is there is no other Google right
being used as being. apologies if he is being. duck duck though they're doing research. But right where else do you go
if you're going to search for images I don't know where, but this is. But there's something about either the data, the
algorithm or both. That exaggerates the stereotypes. Now, I just have a few more slides. If you do find this topic
interesting, this report is really, really good the brookings institution is it's a think tank ABC thing. And they in
2019 they gathered professionals from all across tech from government from academia, to put together a set of
guidelines. For how to detect and mitigate algorithmic bias and a lot of what I talked about in this in this lecture
comes from this report but there's a lot more in there as well, and they give really. Constructive clear guide
guidelines on what companies and institutions should do so, these are some of those recommendations. and the first thing
they come out and say that we need to update our laws are laws are way out of date in this country for dealing with
issues of privacy and bias. And impact the operators of algorithm so like the google's the amazons the facebook's they
need to develop advise impact stations so like sort of like a. No equity statement on so by or something or or
university it's like they need to have a statement about how they think about it, handle bias. They should build diverse
teams across the algorithm development cycles, so this is not just software engineers, this is HR and all the different
and scientists and. Anyone who's involved in the algorithm like assessing the algorithm the outputs like build diverse
teams incorporate all those perspectives into the process itself. And subject yourself to. Financing company to regular
audits regularly audit. Right now, there are no rules about this, but it's like for companies, please, please audit, so
that you can lower the accuracy and increase the fairness of your algorithms right. down to work. This is what we need,
but I don't think we can rely on companies self policing themselves right. And then, this last one is was interesting,
they must rely on cross functional work teams and experience, so this is like you know you would think that only
software engineers are involved in building an algorithm. But you should have sociologists statistician psychologists,
who should have diverse expertise all involved in this algorithm development cycle developing algorithms is not just
engineering. Especially because people. increase the agency of people and then designing monitoring of algorithms like
to have your customers agency or. Now, there should be regulatory sandbox so there's but there's you know there's
obviously going to be pushed back companies will come back and say, well, how are we supposed to innovate, if we have to
be afraid of all these things well. They recognize that as well, there should be regulatory so called sand boxes and
safe harbors so in case they you know made mistakes they're not going to get slapped with huge fines, but they should
fix the mistakes. And then, finally, the consumers need better algorithmic letters I mean this lecture admittedly a
little bit dry. The content can be presented in a very dry way. But that's what this is about like understanding,
fundamentally, what algorithms are how they impact our lives, like what are the these these concepts like fans and
accuracy and things like you can. You don't need to be trained as computer scientists or a statistician to understand
that stuff. But we are clearly influenced, to a degree in candy they appreciate now you can't even see by these factors.
And so that was. Another do that, except for make classes and teach people. This is my last slide and. One of the most
Melissa and my favorite hobbies are philosophical rabbit holes. And so i'm going to put this out there um. And these are
my opinions we can argue about them, if you like, but. I do argue that data is you know quote unquote true to some
extent their observations of the world. They may be flawed. But there there's some there's some truth unless data is
just completely fabricated totally biased there's some truth. But of course the problem that we're dealing with is. The
world that we have is not the world that we want in all respects. But, strictly speaking, if we go and unbiased our data
if we tweak our features, what are we doing we are altering our algorithms data to obtain the desired result. Does that
sound Okay, and like science. Like in the lab you don't change you don't design your experiments well you shouldn't
design your experiments in such a way to just produce a desired result that's bad science that's bias. But that's
exactly what we need to do right so by influencing data and algorithms to mitigate these biases we make these changes
and they'll make changes to create a world that doesn't exist. and has never existed as far as I know. So, whose world
they're recreating. who lives in that world. Who gets to decide what that world looks like. All of us, I mean that
doesn't sound like very practical approach. i'm not saying it shouldn't be but like good luck, making that happen, I
mean what was Winston churchill's famous for saying. Democracy is the worst form of government, except for all the other
ones that have been tried from time to time. Like.

**no speaker (01:24:30.390):** yeah.

**Adam Labadorf (01:24:34.050):**  I so if we're going to employ these tactics, we have to do it very carefully. law of
unintended consequences right. which, of course, not to say, I think it shouldn't be done, of course, you don't know how
to do it when you have to. Think about it. Last semester I got to protect them from students on this slide one of them,
thought it was really depressing, and the other ones thought it was really hopeful. What do you guys think. Does this
slide make you feel yucky. So. So.

**no speaker (01:25:39.990):** Really we're not willing to. Massive.

**Adam Labadorf (01:25:44.760):**  Ai get started, as I sold event.

**no speaker (01:25:49.590):** date. shouldn't be used to be more time to gather.

**Adam Labadorf (01:25:56.160):**  More therapy, so that everyone's laughing before the festival. That we know the site
little light on there, and I will be fine.

**no speaker (01:26:08.940):** You implement it so.

**Adam Labadorf (01:26:14.340):**  So you're saying we shouldn't hold off on. letting Google provide search results
until we have more data. Well, I. think it will be just as with laying on here. Oh next week we'll talk all about that.
How many of you felt hopeful by this idea.

**no speaker (01:26:46.830):** Yes.

**Adam Labadorf (01:26:49.920):**  Nothing gets into the speed at the very least, acknowledging all of the biases that
can either way they buy them from your job or by changing your diet coke out versus advice I think that's an interesting
paradox. And when people are are using these algorithms hopefully they're starting to receive some of this training on
how to. Better approach there they're done so that eliminates some bias, he said, so I guess like talking about learning
about it is helpful and hopefully something that's happening and people who are actively engaging with this technology
know. Though that I mean. Oh. let's see that i'm trying to remember from the brookings report they identified
stakeholders operators for one of the stakeholders, they are the google's the aws like the companies. they're not the
ones who interact with their products can really. Consumers, just like that, at least in their and their formulation. Do
consumers, how much this is, I don't know the answer to this question how much power do you think consumers have to
influence companies to do this. I mean you know I personally am Facebook anymore, because I was not comfortable with
coming to see us by also know that it doesn't even matter what like i'm not actively on paper and on people I think my
data um so I need to not feel like a little bit, or is it not optimistic. optimistic in the fact that there's people
that are talking about this right, and even if it's not enough marks everywhere. Trying to this idea, there are no
people that's like a bar and defensiveness that I didn't like having nobody from the difference. um but I know that I
can't convince Facebook or Google stop doing that you're like me personally and maybe if there's an outcry early you
know something is you know confessional hearing for people actually are they talking about me like the best very
optimistic it's. The first one, there was one recently where they were a bit more sense of this stuff um any other
people actually make decisions to actually push them trying to do something that might not change their actual opinion
on this, but they certainly combined with regulation. On something done right so Europe ggp car so order this up yeah so
privacy privacy thing camera what's called these huge years ago. nope that's a 20 14%. GDP honors in. general data
protection regulation yeah preference of personal data of individuals and the email be processed and transfer. It has
pretty far reaching effects like does it do to you know I don't why suddenly are there, all these like cookie things on
web web pages, it seems like all of a sudden every website now has that you have to click on something or figure out how
to make it go away or something with. their funding and you approve it. right, of course, especially if you're on mobile
like this thing is big enough so that you can actually read the thing unless you actually click it, I agree, Joseph not
just. But if tech didn't have to do that, they wouldn't and in this country they well they don't have je je PR and so I
was wondering if anyone knew was was a law passed recently that requires that in the US or like, why are they doing it.
Because they can control that like they can control aware of what you see this, and we have been for your resided
whenever. Something that talks about the children's online privacy protection but zte relevant. That might be. weird
things happen like they have to do weird things with law, sometimes to get them the past right like they have to game,
the system. Because if they were just like you know the cookie law probably wouldn't fly, but it has something to do
with protecting children it's much, much more palatable for. A congressperson to to put a name on.

**no speaker (01:31:40.620):** It.

**Adam Labadorf (01:31:51.330):**  Alright well that's that's all that I have for today, so if you mean any final
thoughts on this because i'm not going to not be talking about in the President, talking about data and healthcare next
week, which is a little bit of a heavy week so. very interesting branch and heavy. See you Tuesday.

**Felicity Crawford (01:32:19.890):**  boy this this lecture always makes me think about this application.

**Adam Labadorf (01:32:25.200):**  Mostly.

**no speaker (01:32:26.220):** Okay.

**Adam Labadorf (01:32:27.570):**  So so yeah.

**Felicity Crawford (01:32:29.100):**  I said this lecture always makes me think about the logical, the application of
your logical your logic in presenting algorithmic bias. Or does this apply in education, obviously supply base, based on
the values that we hold as a nation, so I i'm still thinking about it than I really grateful for this I haven't had
another opportunity to listen.

**Adam Labadorf (01:32:55.080):**  Okay, thanks for city yeah I try to keep a conceptual know there's. This there's
another version of this talk, which is very technical, which I think point right so.

**Felicity Crawford (01:33:07.560):**  it's really insightful and so. yeah i'm thinking about it and thinking about this
application beyond. You know, education. So thanks thanks thanks again.

**Adam Labadorf (01:33:22.200):**  For happy to chat about it.

**Felicity Crawford (01:33:24.780):**  All right, take care.

**Adam Labadorf (01:33:27.480):**  bye bye.
