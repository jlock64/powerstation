# static-chekcer
this static-checker is used to detect the inefficient API usage that found by our work which includes 9 anti-patterns
1. any? => exists?
2. where.first? => find_by
3. * => *.except(order)
4. each.update => update_all
5. .count => size
6. .map => .pluck
7. pluck.sum => sum
8. .pluck + pluck => SQL UNION
9. if exists? find else create end => find_or_create_by