
# How To Export SVGs For The Web From Illustrator

Something I used to struggle with was exporting SVGs from Illustrator. Our designers make these great comps for us to code up. But what's the best way to take their vector files and convert them into an optimized SVG on the web?

Before sitting down to figure all this out, I'll be honest: I had no idea what the right steps were. Adobe Illustrator has not one, not two, but three different ways to save an SVG! Each one opens up a different set of options and selectors.

I'm not kidding. There's literally three different SVG export screens in Adobe Illustrator.

I want to be clear. I'm not bashing Adobe for having these three different methods. There are actually valid reasons for having three because they each do different things. If you're a designer, you may want to save your SVG in a format that preserves your guides. You don't care about file size. You wouldn't follow these steps at all.

But if you're happier writing code and get anxious at the idea of opening Illustrator, let's walk through the optimal path for getting an SVG into a format that is optimized for use on the web.

## File > Export > Export As…
This is your golden path.

Don't be fooled by the Save for Web option. You want to go with File > Export > Export As… Name your file and choose SVG as the format. It may seem like you're about to save the image without the ability setting any options once you click Export. That button actually opens a new window before the file saves.

In most cases, these will be the options you'll want to check. We'll go into why below, but if you're looking for the tl;dr version, mimic what you see here and you'll be good to go:

Export window

##Styling
You'll almost always want to choose presentation attributes. If we have an SVG that is black but want it to be white in a hover state, we'd use CSS to change the color. If the black color is saved as presentation attributes, it's easier to define that new color because CSS always overwrites presentation attributes. Specificity can be our friend!

Inline style or internal CSS are useful if we have a giant SVG that we're trying to optimize in some way. But 99% of the time, presentation attributes is the option you'll want.

##Font
Choosing font is the much more efficient option, especially on bigger images. The only reason you'd want to choose convert to outlines is if you were using an obscure font (maybe in a client logo) or you were having trouble with letters displaying correctly in your export.

Convert to outlines changes your letters from a font to vectors. You may solve a display issue but you're taking a performance hit and likely breaking accessibility guidelines. Like presentation attributes above, 99% of the time you'll want to go with font as your option here.

##Images
If you are using a raster graphic (like a JPG) in your SVG, you have two options. Choosing link means the raster graphic will live in its own file somewhere else. Choosing embed will make it part of the SVG. There's no real performance difference either way since the file still has to be loaded. But linking keeps your SVG and non SVG components separate and easier to read. This one is personal preference. I like to embed it unless it's a raster graphic I'm reusing elsewhere.

##Object IDs
This is what is used by CSS or JS to target parts of the image for manipulation. Minimal is usually the best choice. Unique will create long strings of text to ensure everything is different. But it's a pain to copy those strings to CSS or JS. If you've named all your layers in Illustrator, you can choose layer names to have those be the IDs.

Since I usually don't need to be able to target every single aspect of an SVG, I go with minimal and update any classes I do use with a find/replace in my IDE. You could just as easily do this in Illustrator but I'm more comfortable editing code than editing an image.

Minimal is great for file size, but if you have multiple SVGs with minimal class names, you're going to end up styling things you didn't mean to because you have duplication. Hence why I go with minimal and then modify as I need to use them.

##Decimal
2 is usually the best choice. If you make the number smaller, you're removing precision of your vectors. If you make the number bigger, you're adding precision but also adding to the file size.

##Minify
Yes, please.

##Responsive
It might make logical sense to turn this on. But we actually want to leave it off. If we check this box, our SVG won't have any width or height on it. Until we add a width and height with CSS, our SVGs won't know what to do. In a lot of cases, they will fill as much space as possible. By turning off responsive, we are adding a width and height to the base SVG. Luckily, if we also define a width and height in our CSS, it will override what is defined in the SVG itself.

Now What? Now that you have your SVGs optimized and ready for use on the web, you're all set to use them. Unlike other image files, there's a couple different ways to get your vectors onto your page. I gave a talk at Connect.Tech in 2017 about best practices on SVG implementation. Shameless plug: you can watch it here.
