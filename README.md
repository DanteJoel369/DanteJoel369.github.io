# Setup: free site on GitHub Pages

## Part 1: Publish the site
1. Create a free account at github.com. Your username becomes your address.
2. Click New repository. Name it exactly `dantejoel369.github.io` and make it Public.
3. Click "uploading an existing file", drag in everything in this folder (index.html, robots.txt, sitemap.xml, llms.txt), and commit.
4. Go to Settings > Pages. Set Source to "Deploy from a branch", branch `main`, folder `/ (root)`. Save.
5. After a minute or two the site is live at https://dantejoel369.github.io (no hosting or domain fee).
6. Find and replace `dantejoel369` and "Digital Dreams" in all four files with your real details.
7. Create a free form on Formspree or Buttondown and paste its URL into the subscribe form in index.html.

A custom domain (yourname.com) costs money and is optional. The github.io address is free.

## Part 2: Install the agents (on your own computer)
The agents are text files that Claude Code reads, so they can't be installed from claude.ai chat. You need Git and Claude Code on your computer.

    git clone https://github.com/msitarzewski/agency-agents.git
    cd agency-agents
    ./scripts/install.sh --help
    ./scripts/install.sh --tool claude-code --division marketing

Use `--help` to see the exact division and agent options in the current version. Installing 5 to 10 agents works better than installing all of them, so start with Content Creator, SEO Specialist, Social Media Strategist, Email Marketing Strategist and AI Citation Strategist, then add the rest.
The project also offers a desktop installer app if you prefer not to use the terminal.

Then, in Claude Code inside your site folder, ask for example: "Use the SEO Specialist agent to review index.html."
