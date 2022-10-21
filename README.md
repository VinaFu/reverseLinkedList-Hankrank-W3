# reverseLinkedList-Hankrank-W3



        def reverse(llist):
            # Write your code here
            node, end = llist, None              // value and the end
            while node:
                node.prev, node.next = node.next, node.prev
                                                // form the double direct node
                end = node                      // first would be the value
                node = node.prev                // ahead one would be prev.

            return end
