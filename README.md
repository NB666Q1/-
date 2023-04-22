from textblob import TextBlob

def calculate_goodwill_score(description):
    blob = TextBlob(description)
    sentiment_score = blob.sentiment.polarity
    goodwill_value = (sentiment_score + 1) * 50
    return goodwill_value

# 示例调用
description = "小明很友善，经常帮助别人。"
goodwill_value = calculate_goodwill_score(description)
result = f"您对{name}的好感度为{goodwill_value:.2f}。"
print(result)



# -
根据用户描述进行好感度计算，需要安装 TextBlob 库
