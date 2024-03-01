# Generative Diagram Documentation
<br>
This is an interactive documentation for research and work processes. It is a small tool for presenting workflows and outcome but also for showcasing roads not taken. The documentation is generated from a Markdown file that can be edited to reflect the structure of your project. 
<br>
<br>
In the markdown file you can also use the JSON structure to define the diagram. To create levels add them to <code>children:[]</code> in the <code>data</code> object. The levels need a distinct name (e.g. <code>L0, L1, ...</code>). In <code>content</code> you can define the content you want to show (even images). To link item in a new level to a parent use the identifier of the parent in the <code>imports</code> array (data.L0.1, data.L0.2, ...).
---
{
    "name": "data",
    "children": [
        {
            "name": "L0",
            "level": 0,
            "children": [
                {
                    "name": "1",
                    "type": "topic",
                    "content": "Topic",
                    "imports": []
                },
                {
                    "name": "2",
                    "type": "process",
                    "content": "Process",
                    "imports": []
                },
                {
                    "name": "3",
                    "type": "question",
                    "content": "Question",
                    "imports": []
                },
                {
                    "name": "5",
                    "type": "input",
                    "content": "Input",
                    "imports": []
                },
                {
                    "name": "6",
                    "type": "result",
                    "content": "Result",
                    "imports": []
                }
            ]
        },
        {
            "name": "L1",
            "level": 1,
            "children": [
                {
                    "name": "4",
                    "type": "output",
                    "content": "Output",
                    "imports": ["data.L0.1", "data.L0.3", "data.L0.6"]
                }
            ]
        }
    ]
}
-----
# Two

This is an interactive documentation for research and work process.

---
{
    "name": "data",
    "children": [
        {
            "name": "L0",
            "level": 0,
            "children": [
                {
                    "name": "1",
                    "type": "topic",
                    "content": "Topic",
                    "imports": []
                },
                {
                    "name": "2",
                    "type": "process",
                    "content": "Process",
                    "imports": []
                },
                {
                    "name": "3",
                    "type": "question",
                    "content": "Question",
                    "imports": []
                },
                {
                    "name": "5",
                    "type": "input",
                    "content": "Input",
                    "imports": []
                },
                {
                    "name": "6",
                    "type": "result",
                    "content": "Result",
                    "imports": []
                }
            ]
        },
        {
            "name": "L1",
            "level": 0,
            "children": [
                {
                    "name": "4",
                    "type": "result",
                    "content": "Output",
                    "imports": ["data.L0.1", "data.L0.2", "data.L0.3", "data.L0.6"]
                }
            ]
        },
        {
                        "name": "L2",
            "level": 0,
            "children": [
                {
                    "name": "4",
                    "type": "result",
                    "content": "Output",
                    "imports": ["data.L0.1"]
                }
            ]
        }
    ]
}

