# Slides in Markdown for teaching at ICAI

This project is just an example based on this library: [mkslides](https://github.com/MartenBE/mkslides).

## What is this about?

In a world where we are using Markdown more and more, especially taking into account that LLMs can read Markdown easily, this repository shows an example configuration for generating slides with Markdown.

## How to execute

The `mkslides` library allows two different execution modes, by folder and file. Here, the example that we have drafted is to always follow the execution by folder. Specifically, we have created the example to have a folder (in this case `src`) that contains all the files needed for a set of slides. 

We have decided in this template to put a folder for each set of slides so they are more independent, and each set of slides is something that you can edit without having to worry about anything else.

Now, to visualize the slides you just have to follow the following commands:

```bash
# Install libraries
uv sync

# Serve slides
cd src
mkslides serve .
```

This creates a html visualization in `localhost:8000`. If you want to use `pdf` you can just add the suffix `?print-pdf` having `localhost:8000/?print-pdf`.

This is prepared, so slides are generated from inside the folder. This is why slides have to be served as `mkslides serve .`. If you want to build the html for later use you will have to use the `build` command in the same way:

```bash
mkslides build .
```

Then, you can just replicate `src` folder for each set of slides you need.

## Resources

If you want to explore more about generating slides with markdown we recommend that you check the actual library that we have used to generate these slides besides more resources we have found:

- [Mkslides Documentation](https://github.com/MartenBE/mkslides)
- [Mkslides Example](https://martenbe.github.io/mkslides/)
- [Mkslides Examples with HOGENT theme](https://github.com/HoGentTIN/hogent-markdown-slides)

## AI Disclaimer

The use of AI that you will find in this repository is only auxiliary. Here AI has only helped debug and draft some documentation when online documentation might not be enough. AI has not been used to generate the whole files or to vibe code in any sense. The final purpose of this repository is learning, which we believe is against using AI for everything without spending the time to actually learn from what you are building.  
