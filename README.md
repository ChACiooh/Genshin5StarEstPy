# Genshin5StarEstimation Python Version
Program which estimates probabilities of pick 5 star characters that you focused on in n tries on Genshin Impact.

## Developer
- CSE major who loves Hu-Tao in Genshin Impact so much.
- contact : @7A4ys(twitter) / email:honoki47@gmail.com

## Purpose
People who want to pick new 5 star character always have money issue. So, when people know how much money they have and consider how many they want to pick, this will be helpful.

## Note
It is necessary to make directories: ./result_txt and ./result_xls

## Usage
1. input stack value of your gacha (1 ~ 89)
2. input your state whether now is in 100% pick up or not. (y/n)
3. input gachas you can try.

## Output = probability of picking n characters in k tries(k: output %).
- n_basic_s.txt : basical probs with s stack you provided.
- n_pick_s.txt : first gacha with s stack gives pick-up character obviously, and probs based on it.

## Principle
Previous result of the gacha affects next gacha. And from 74th to 89th tries in each stage of gacha have another probability. Of course, 100% on k >= 90, k is the number of tries. It says Dynamic Programming needed because such system has previous result affects next output. You can consider recursive algorithm but it has the time complexity of O(N^M). However, DP algorithm changes it into O(N\*M\*K), N and K is very less than M.

## After
These python codes will be uploaded on a web site.
