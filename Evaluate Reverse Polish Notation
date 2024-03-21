class Solution {
    public int evalRPN(String[] tokens) {
        Stack<Integer> st = new Stack<>();
        
        for (int i = 0; i < tokens.length; i++){
            if (tokens[i].equals("+")){
                st.push(st.pop() + st.pop());
            } else if (tokens[i].equals("-")){
                st.push(-(st.pop() - st.pop()));
            } else if (tokens[i].equals("*")){
                st.push(st.pop() * st.pop());
            } else if (tokens[i].equals("/")){
                int num = st.pop();
                st.push(st.pop() / num);
            } else{
                st.push(Integer.parseInt(tokens[i]));
            }
        }

        return st.pop();
    }
}
