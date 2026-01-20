```markdown
# Mobile Automation Tool Documentation

## MadHub's Powerful Automation Features

MadHub's powerful automation features leverage advanced Android APIs to enable efficient and effective mobile automation across platforms like Facebook, Instagram, and TikTok. This tool is designed to operate seamlessly on real Android devices, cloud phones, or emulators, allowing for 24/7 automated operations without the need for constant supervision. 

### Featured Capabilities

One of the standout features of MadHub is the **Facebook Account Warm-Up**. This powerful technical feature simulates real user behavior by browsing through homepage feeds and video pages while intelligently skipping ad videos. It supports various interaction types, including likes and comments, and allows users to configure interaction probability and execution probability distributions. This functionality is essential for improving account activity and weight, significantly reducing the risk of account bans, and establishing trustworthiness for new or existing accounts.

Another notable feature is **Facebook Auto-Reply**, which provides automated responses to unread Facebook messages. This feature ensures timely communication with users by replying to messages 24/7 and supports configurable settings, including operation intervals and message templates. 

### Technical Usage

#### Facebook Account Warm-Up

To utilize the **Facebook Account Warm-Up** feature:
1. **Set Interaction Probability**: Define how often the bot should like or comment on posts.
2. **Configure Execution Probability**: Adjust the likelihood of various browsing activities, allowing you to simulate authentic user engagement effectively.

**Example Usage**:
```java
MadHub facebookAutomation = new MadHub();
facebookAutomation.startFacebookAccountWarmUp();
facebookAutomation.setInteractionProbability(70); // 70% chance to like posts
facebookAutomation.setExecutionProbability(60); // 60% chance to comment
```
This configuration allows for a balanced approach to automating user interactions, enhancing the natural appearance of account activity.

#### Facebook Auto-Reply

For the **Facebook Auto-Reply** feature:
1. **Input Mode**: Choose to reply with pre-defined messages or random messages from a file.
2. **Set Operation Interval**: Determine how often the bot should check for unread messages (e.g., every 5 minutes).

**Example Usage**:
```java
MadHub facebookAutomation = new MadHub();
facebookAutomation.startFacebookAutoReply();
facebookAutomation.setOperationInterval(5); // Check messages every 5 minutes
facebookAutomation.setReplyMode("file"); // Use messages from a designated file
```
This setup allows for efficient message management, ensuring that you never miss a customer inquiry.

### Configuration Examples

MadHub provides flexible configuration options for both features:

#### Facebook Account Warm-Up Configuration
- **Interaction Probability**: Adjust the likelihood of engagement (0-100%).
- **Execution Probability Distribution**: Define how different types of interactions are executed (e.g., likes vs. comments).

For example, to set a 50% interaction probability and a custom execution distribution of 80% likes and 20% comments:
```java
facebookAutomation.setInteractionProbability(50);
facebookAutomation.setExecutionProbabilityDistribution(80, 20);
```

#### Facebook Auto-Reply Configuration
- **Operation Interval**: Set how often the bot checks for new messages.
- **Message Templates**: Define different templates for replies.

To configure:
```java
facebookAutomation.setOperationInterval(10); // Check every 10 minutes
facebookAutomation.addMessageTemplate("Thank you for reaching out!"); // Add reply templates
facebookAutomation.addMessageTemplate("We're here to help!"); // Another template
```

## Conclusion

In summary, MadHub provides a comprehensive and robust solution for mobile automation needs, particularly for social media operations. With features like **Facebook Account Warm-Up** and **Facebook Auto-Reply**, users can enhance their engagement strategies and maintain effective communication with their audience. The flexibility and configurability of these features empower users to tailor their automation strategies, fostering growth and increasing operational efficiency. Explore MadHub's capabilities today to elevate your mobile automation processes.
```
