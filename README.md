# EmotionMarket-Emotionsbasiertes-Marketing-mit-KI
EmotionMarket nutzt Emotionserkennung und generative KI, um personalisierte Marketingkampagnen zu erstellen, die auf die Gefühle und Vorlieben der Zielgruppe zugeschnitten sind.
import random

def recognize_emotion(text):
    """Placeholder function for emotion recognition from text.
    In reality, this would be replaced with an actual NLP model.
    """
    emotions = ['happy', 'sad', 'angry', 'fearful', 'surprised']
    # This is a placeholder. In a real application, analyze the text.
    return random.choice(emotions)

def generate_marketing_message(emotion):
    """Generates a marketing message based on the recognized emotion."""
    messages = {
        'happy': "We're glad you're feeling joyful! Celebrate with our special offer.",
        'sad': "Feeling down? Our product might just be the pick-me-up you need.",
        'angry': "We understand life's frustrations. Our service can help ease your day.",
        'fearful': "It's okay to feel unsure. Our product offers the security you're looking for.",
        'surprised': "Surprised? So are we, with these amazing deals just for you!"
    }
    return messages.get(emotion, "Discover how our product can match your mood today!")

def main():
    print("Welcome to EmotionMarket Demo")
    text = input("How are you feeling today? Share a bit about your day: ")
    
    emotion = recognize_emotion(text)
    print(f"\nDetected Emotion: {emotion.capitalize()}")
    
    message = generate_marketing_message(emotion)
    print(f"\nCustomized Marketing Message:\n{message}")

if __name__ == "__main__":
    main()
