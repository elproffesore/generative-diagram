# Generative Diagram Documentation

This is an interactive documentation for research and work processes. It is a small tool for presenting workflows and outcome but also for showcasing roads not taken. The documentation is generated from a Markdown file that can be edited to reflect the structure of your project. 

## Usage
In the markdown file you can also use the JSON structure to define the diagram. To create levels add them to <code>children:[]</code> in the <code>data</code> object. The levels need a distinct name (e.g. <code>L0, L1, ...</code>). In <code>content</code> you can define the content you want to show (even images). To link item in a new level to a parent use the identifier of the parent in the <code>imports</code> array (data.L0.1, data.L0.2, ...).

## Installation

1. Edit the content.md file to reflect the structure of your project.
2. Run webserver with the contents.

## Showcase

![Demovideo](./media/demonstration.gif)