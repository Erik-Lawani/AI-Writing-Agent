A multi-agent writing system built with AutoGen that demonstrates collaborative AI agents working together to create structured content. This project showcases how specialized AI agents can be orchestrated to handle complex writing tasks through role-based collaboration.

## Features

- **Multi-Agent Architecture**: Two specialized agents working in tandem
  - **Planner Agent**: Creates structured outlines for blog posts and articles
  - **Writer Agent**: Transforms outlines into comprehensive written content
- **Intelligent Handoff System**: Agents seamlessly pass work between each other using handoff messages
- **Flexible Termination**: Smart termination conditions that stop the workflow when content is complete
- **Streaming Output**: Real-time display of agent interactions and content generation

## How It Works

1. **Planning Phase**: The Planner Agent receives a topic and creates a structured outline with key sections (Introduction, Background, Key Insights, Challenges, Conclusion)
2. **Handoff**: The planner signals completion and hands off to the writer with a handoff message
3. **Writing Phase**: The Writer Agent takes the outline and generates detailed content for each section
4. **Termination**: The system automatically stops when the writer completes the conclusion section

## Technical Implementation

- Built with **AutoGen** for multi-agent coordination
- Uses **OpenAI GPT-4o** for content generation
- Implements custom agent classes inheriting from `BaseChatAgent`
- Features intelligent termination conditions using `TextMentionTermination` and `HandoffTermination`
- Console-based UI for real-time interaction monitoring

## Usage

The system can be easily extended to handle different types of writing tasks by modifying the agent prompts and outline structures. Simply provide a topic and watch as the agents collaborate to create well-structured, comprehensive content.

## Example Output

For a topic like "The impact of AI on education", the system will:
1. Generate a structured outline covering all key aspects
2. Create detailed content for each section
3. Provide a complete, publication-ready article

This project demonstrates the power of multi-agent systems in content creation and serves as a foundation for building more complex collaborative AI workflows.
